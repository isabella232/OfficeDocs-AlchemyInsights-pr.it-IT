---
title: Risolvere il problema del PRT
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/04/2020
ms.locfileid: "49571970"
---
# <a name="troubleshoot-prt-issue"></a><span data-ttu-id="9b8a4-102">Risolvere il problema del PRT</span><span class="sxs-lookup"><span data-stu-id="9b8a4-102">Troubleshoot PRT issue</span></span>

<span data-ttu-id="9b8a4-103">Affinché tutti i dispositivi vengano completati come autenticati, è necessario che siano completamente registrati e in grado di acquisire un token di aggiornamento primario (PRT).</span><span class="sxs-lookup"><span data-stu-id="9b8a4-103">For any device to complete getting authenticated, it must be fully registered and in good state and able to acquire a Primary Refresh Token (PRT).</span></span>

<span data-ttu-id="9b8a4-104">Il processo di registrazione ibrido di Azure AD join richiede che i dispositivi si trovino in una rete aziendale.</span><span class="sxs-lookup"><span data-stu-id="9b8a4-104">The hybrid Azure AD join registration process requires devices to be on a corporate network.</span></span> <span data-ttu-id="9b8a4-105">Funziona anche su VPN, ma ci sono alcune avvertenze.</span><span class="sxs-lookup"><span data-stu-id="9b8a4-105">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="9b8a4-106">Sono stati ascoltati i clienti che hanno bisogno di assistenza per la risoluzione dei problemi del processo di registrazione del join di Azure AD in modalità remota.</span><span class="sxs-lookup"><span data-stu-id="9b8a4-106">We’ve heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote-work circumstances.</span></span> <span data-ttu-id="9b8a4-107">Di seguito viene indicato un problema relativo a ciò che accade sotto la cappa durante il processo di registrazione.</span><span class="sxs-lookup"><span data-stu-id="9b8a4-107">Here’s a breakdown of what’s happening ‘under the hood’ during the registration process.</span></span>

<span data-ttu-id="9b8a4-108">**Ambiente di autenticazione cloud (tramite l'autenticazione hash della password di Azure AD o pass-through)**</span><span class="sxs-lookup"><span data-stu-id="9b8a4-108">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="9b8a4-109">Questo flusso di registrazione è noto anche come "sincronizzazione join".</span><span class="sxs-lookup"><span data-stu-id="9b8a4-109">This registration flow is also known as “Sync Join”.</span></span>

1. <span data-ttu-id="9b8a4-110">Windows 10 consente di individuare un record SCP al momento dell'accesso dell'utente al dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9b8a4-110">Windows 10 discovers an SCP record upon user logging on to the device.</span></span>
    1. <span data-ttu-id="9b8a4-111">Il dispositivo tenta innanzitutto di recuperare le informazioni sul tenant dall'SCP sul fianco del client nel registro di sistema [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span><span class="sxs-lookup"><span data-stu-id="9b8a4-111">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="9b8a4-112">Per ulteriori informazioni, vedere questo [documento](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span><span class="sxs-lookup"><span data-stu-id="9b8a4-112">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    2. <span data-ttu-id="9b8a4-113">In caso di esito negativo, il dispositivo comunica con Active Directory locale (AD) per ottenere informazioni sul tenant dal punto di connessione del servizio (SCP, Service Connection Point).</span><span class="sxs-lookup"><span data-stu-id="9b8a4-113">If it fails, the device communicates with on-premises Active Directory (AD) to get tenant information from Service Connection Point (SCP).</span></span> <span data-ttu-id="9b8a4-114">Per verificare SCP, fare riferimento a questo [documento](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span><span class="sxs-lookup"><span data-stu-id="9b8a4-114">To verify SCP, please refer to this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span> 

> [!NOTE]
> <span data-ttu-id="9b8a4-115">Si consiglia di abilitare SCP nell'annuncio e di utilizzare solo SCP sul fianco del client per la convalida iniziale.</span><span class="sxs-lookup"><span data-stu-id="9b8a4-115">We recommend enabling SCP in the AD and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="9b8a4-116">Windows 10 tenta di comunicare con Azure AD nel contesto di sistema per autenticarsi con Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9b8a4-116">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span> <span data-ttu-id="9b8a4-117">È possibile verificare se il dispositivo può accedere alle risorse Microsoft con l'account di sistema utilizzando lo script di connettività di registrazione del dispositivo di test.</span><span class="sxs-lookup"><span data-stu-id="9b8a4-117">You can verify if the device can access Microsoft resources under the system account by using the Test Device Registration Connectivity script.</span></span>

3. <span data-ttu-id="9b8a4-118">Windows 10 genera un certificato autofirmato e lo archivia sotto l'oggetto computer in Active Directory locale.</span><span class="sxs-lookup"><span data-stu-id="9b8a4-118">Windows 10 generates a self-signed certificate and stores it under the computer object in on-premises AD.</span></span> <span data-ttu-id="9b8a4-119">Questo richiede la linea di vista per il controller di dominio.</span><span class="sxs-lookup"><span data-stu-id="9b8a4-119">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="9b8a4-120">Un oggetto Device che dispone di un certificato viene sincronizzato con Azure ad tramite Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="9b8a4-120">A device object that has a certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="9b8a4-121">Il ciclo di sincronizzazione è ogni 30 minuti per impostazione predefinita, ma dipende dalla configurazione di Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="9b8a4-121">Sync cycle is every 30 minutes by default, but it depends on configuration of Azure AD Connect.</span></span> <span data-ttu-id="9b8a4-122">Per ulteriori informazioni, fare riferimento a questo [documento](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span><span class="sxs-lookup"><span data-stu-id="9b8a4-122">For more information, please refer to this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="9b8a4-123">In questa fase, è necessario essere in grado di visualizzare il dispositivo soggetto nello stato in sospeso in dispositivo Blade del portale di Azure.</span><span class="sxs-lookup"><span data-stu-id="9b8a4-123">At this stage, you should be able to see the subject device in “Pending” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="9b8a4-124">Al successivo accesso utente a Windows 10, la registrazione sarà completata.</span><span class="sxs-lookup"><span data-stu-id="9b8a4-124">At the next user login to Windows 10, the registration will be completed.</span></span> 

> [!NOTE]
> <span data-ttu-id="9b8a4-125">Se si è in VPN e un processo di accesso di disconnessione termina la connettività del dominio, è possibile attivare la registrazione manualmente:</span><span class="sxs-lookup"><span data-stu-id="9b8a4-125">If you're on VPN and a logoff-login process terminates the domain connectivity, you can trigger registration manually:</span></span>
 1. <span data-ttu-id="9b8a4-126">Emettere un/join di dsregcmd localmente su prompt di amministratore o in remoto tramite PSExec al PC.</span><span class="sxs-lookup"><span data-stu-id="9b8a4-126">Issue a dsregcmd /join locally on admin prompt or remotely via PSExec to your PC.</span></span> <span data-ttu-id="9b8a4-127">Ad esempio, PsExec-s \\ win10client01 cmd, dsregcmd/join</span><span class="sxs-lookup"><span data-stu-id="9b8a4-127">For example, PsExec -s \\win10client01 cmd, dsregcmd /join</span></span>

 2. <span data-ttu-id="9b8a4-128">Per ulteriori informazioni sui problemi di join ibrido, vedere [risolvere i problemi relativi ai dispositivi](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span><span class="sxs-lookup"><span data-stu-id="9b8a4-128">For more details on Hybrid Join issues, see [Troubleshoot devices Issue](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span></span>
