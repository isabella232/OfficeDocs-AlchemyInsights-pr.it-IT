---
title: Dispositivo in stato in sospeso
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/11/2020
ms.locfileid: "49652189"
---
# <a name="device-in-pending-state"></a><span data-ttu-id="2bfa0-102">Dispositivo in stato in sospeso</span><span class="sxs-lookup"><span data-stu-id="2bfa0-102">Device in pending state</span></span>

<span data-ttu-id="2bfa0-103">**Prerequisiti**</span><span class="sxs-lookup"><span data-stu-id="2bfa0-103">**Prerequisites:**</span></span>

1. <span data-ttu-id="2bfa0-104">Se si stanno configurando le registrazioni del dispositivo per la prima volta, assicurarsi di aver esaminato l' [Introduzione alla gestione dei dispositivi in Azure Active Directory (Azure ad)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) che guiderà l'utente su come ottenere i dispositivi sotto il controllo di Azure ad.</span><span class="sxs-lookup"><span data-stu-id="2bfa0-104">If you are setting up device registrations for the first time, please ensure that you have reviewed [Introduction to device management in Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) that will guide you on how to get devices under the control of Azure AD.</span></span>
2. <span data-ttu-id="2bfa0-105">Se si sta registrando i dispositivi in Azure AD direttamente e si esegue la registrazione in Intune, è necessario assicurarsi di aver [configurato Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) e di disporre della [licenza](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) per prima.</span><span class="sxs-lookup"><span data-stu-id="2bfa0-105">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
3. <span data-ttu-id="2bfa0-106">Assicurarsi di essere autorizzati a eseguire operazioni in Azure Active Directory e Active Directory locale.</span><span class="sxs-lookup"><span data-stu-id="2bfa0-106">Ensure you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="2bfa0-107">Solo un amministratore globale di Azure AD è in grado di gestire le impostazioni per le registrazioni dei dispositivi.</span><span class="sxs-lookup"><span data-stu-id="2bfa0-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="2bfa0-108">Inoltre, se si stanno configurando le registrazioni automatiche in Active Directory locale, è necessario essere un amministratore di Active Directory e AD FS (se applicabile).</span><span class="sxs-lookup"><span data-stu-id="2bfa0-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="2bfa0-109">Il processo di registrazione ibrido di Azure AD join richiede che i dispositivi siano sulla rete aziendale.</span><span class="sxs-lookup"><span data-stu-id="2bfa0-109">The hybrid Azure AD join registration process requires devices to be on corporate network.</span></span> <span data-ttu-id="2bfa0-110">Funziona anche su VPN, ma ci sono alcune avvertenze.</span><span class="sxs-lookup"><span data-stu-id="2bfa0-110">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="2bfa0-111">Sono stati ascoltati i clienti che hanno bisogno di assistenza per la risoluzione dei problemi relativi al processo di registrazione di join di Azure AD in condizioni di lavoro remote.</span><span class="sxs-lookup"><span data-stu-id="2bfa0-111">We have heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote work circumstances.</span></span>

<span data-ttu-id="2bfa0-112">**Ambiente di autenticazione cloud (tramite l'autenticazione hash della password di Azure AD o pass-through)**</span><span class="sxs-lookup"><span data-stu-id="2bfa0-112">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="2bfa0-113">Questo flusso di registrazione è noto anche come "sincronizzazione join".</span><span class="sxs-lookup"><span data-stu-id="2bfa0-113">This registration flow is also known as “Sync Join”.</span></span>

<span data-ttu-id="2bfa0-114">Di seguito viene indicato un guasto di ciò che avviene durante il processo di registrazione:</span><span class="sxs-lookup"><span data-stu-id="2bfa0-114">Here is a breakdown of what happens during the registration process:</span></span>

1. <span data-ttu-id="2bfa0-115">Windows 10 rileva il record SCP (Service Connection Point) quando l'utente esegue l'accesso al dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2bfa0-115">Windows 10 discovers Service Connection Point (SCP) record when the user logs on to the device.</span></span>

    1. <span data-ttu-id="2bfa0-116">Il dispositivo tenta innanzitutto di recuperare le informazioni sul tenant dall'SCP sul fianco del client nel registro di sistema [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span><span class="sxs-lookup"><span data-stu-id="2bfa0-116">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="2bfa0-117">Per ulteriori informazioni, vedere [Document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span><span class="sxs-lookup"><span data-stu-id="2bfa0-117">For more information, see [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    1. <span data-ttu-id="2bfa0-118">In caso di esito negativo, il dispositivo comunica con Active Directory locale per ottenere informazioni sul tenant da SCP.</span><span class="sxs-lookup"><span data-stu-id="2bfa0-118">If it fails, the device communicates with on-premises Active Directory to get tenant information from SCP.</span></span> <span data-ttu-id="2bfa0-119">Per verificare SCP, fare riferimento a questo [documento](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span><span class="sxs-lookup"><span data-stu-id="2bfa0-119">To verify SCP, refer this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span>

    > [!NOTE]
    > <span data-ttu-id="2bfa0-120">Si consiglia di abilitare SCP in Active Directory e di utilizzare solo SCP sul fianco client per la convalida iniziale.</span><span class="sxs-lookup"><span data-stu-id="2bfa0-120">We recommend enabling SCP in the Active Directory and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="2bfa0-121">Windows 10 tenta di comunicare con Azure AD nel contesto di sistema per autenticarsi con Azure AD.</span><span class="sxs-lookup"><span data-stu-id="2bfa0-121">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span>

    <span data-ttu-id="2bfa0-122">È possibile verificare se il dispositivo può accedere alle risorse Microsoft con l'account di sistema utilizzando lo [script di connettività di registrazione del dispositivo di test](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span><span class="sxs-lookup"><span data-stu-id="2bfa0-122">You can verify if the device can access Microsoft resources under the system account by using the [Test Device Registration Connectivity script](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span></span>

3. <span data-ttu-id="2bfa0-123">Windows 10 genera un certificato autofirmato e lo archivia sotto l'oggetto computer in Active Directory locale.</span><span class="sxs-lookup"><span data-stu-id="2bfa0-123">Windows 10 generates self-signed certificate and stores it under the computer object in on-premises Active Directory.</span></span> <span data-ttu-id="2bfa0-124">Questo richiede la linea di vista per il controller di dominio.</span><span class="sxs-lookup"><span data-stu-id="2bfa0-124">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="2bfa0-125">Oggetto Device con certificato ottenuto sincronizzato con Azure ad tramite Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="2bfa0-125">Device object that has certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="2bfa0-126">Il ciclo di sincronizzazione è ogni 30 minuti per impostazione predefinita, ma dipende dalla configurazione di Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="2bfa0-126">Sync cycle is every 30 minutes by default, but it depends on the configuration of Azure AD Connect.</span></span> <span data-ttu-id="2bfa0-127">Per ulteriori informazioni, fare riferimento a questo [documento](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span><span class="sxs-lookup"><span data-stu-id="2bfa0-127">For more information, refer this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="2bfa0-128">In questa fase, è necessario essere in grado di visualizzare il dispositivo soggetto nello stato in **sospeso** in dispositivo Blade del portale di Azure.</span><span class="sxs-lookup"><span data-stu-id="2bfa0-128">At this stage, you should be able to see the subject device in “**Pending**” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="2bfa0-129">Al successivo accesso utente a Windows 10, la registrazione sarà completata.</span><span class="sxs-lookup"><span data-stu-id="2bfa0-129">At the next user login to Windows 10, the registration will be completed.</span></span>

    > [!NOTE]
    > <span data-ttu-id="2bfa0-130">Se si è in VPN e la disconnessione/accesso termina la connettività del dominio, è possibile attivare la registrazione manualmente.</span><span class="sxs-lookup"><span data-stu-id="2bfa0-130">If you are on VPN and logoff/login terminates the domain connectivity, you can trigger registration manually.</span></span> <span data-ttu-id="2bfa0-131">A questo scopo:</span><span class="sxs-lookup"><span data-stu-id="2bfa0-131">To do that:</span></span>
    >
    > <span data-ttu-id="2bfa0-132">Emettere un `dsregcmd /join` prompt di amministratore localmente o in remoto tramite PsExec nel PC.</span><span class="sxs-lookup"><span data-stu-id="2bfa0-132">Issue a `dsregcmd /join` locally on admin prompt or remotely via PSExec to your PC.</span></span>
    >
    > <span data-ttu-id="2bfa0-133">Ad esempio: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span><span class="sxs-lookup"><span data-stu-id="2bfa0-133">For example: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span></span>

<span data-ttu-id="2bfa0-134">Per i problemi comuni relativi alla registrazione del dispositivo di Azure Active Directory, vedere [FAQ sui dispositivi](https://docs.microsoft.com/azure/active-directory/devices/faq).</span><span class="sxs-lookup"><span data-stu-id="2bfa0-134">For common issues with Azure Active Directory device registration, see [Devices FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq).</span></span>
