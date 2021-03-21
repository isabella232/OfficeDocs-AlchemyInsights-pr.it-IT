---
title: Configurare il punto di connessione del servizio (SCP)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 9d733a1a0a3b8d92bdd5477a8978b6fbeede9653
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 03/19/2021
ms.locfileid: "50898063"
---
# <a name="configure-service-connection-point-scp"></a><span data-ttu-id="97253-102">Configurare il punto di connessione del servizio (SCP)</span><span class="sxs-lookup"><span data-stu-id="97253-102">Configure Service connection Point (SCP)</span></span>

<span data-ttu-id="97253-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span><span class="sxs-lookup"><span data-stu-id="97253-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span></span>

- <span data-ttu-id="97253-104">**Motivo**: non è possibile leggere l'oggetto SCP e ottenere le informazioni sul tenant di Azure AD</span><span class="sxs-lookup"><span data-stu-id="97253-104">**Reason**: Unable to read the SCP object and get the Azure AD tenant information</span></span>
- <span data-ttu-id="97253-105">**Risoluzione**: vedere la sezione [Configurare un punto di connessione del servizio](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span><span class="sxs-lookup"><span data-stu-id="97253-105">**Resolution**: Refer to the section [Configure a Service Connection Point](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span></span>


<span data-ttu-id="97253-106">**Piano di azione**</span><span class="sxs-lookup"><span data-stu-id="97253-106">**Action plan**</span></span>

- <span data-ttu-id="97253-107">Verificare se il dispositivo ha ricevuto l'oggetto Criteri di gruppo per la convalida controllata.</span><span class="sxs-lookup"><span data-stu-id="97253-107">Check whether the device has received the GPO for the controlled validation.</span></span>
- <span data-ttu-id="97253-108">Verificare che l'oggetto Criteri di gruppo abbia creato le chiavi del Registro di sistema.</span><span class="sxs-lookup"><span data-stu-id="97253-108">Ensure that the GPO has created the registry keys.</span></span>
- <span data-ttu-id="97253-109">Assicurarsi di aver creato 2 chiavi con l'ID directory e il dominio onmicrosoft.</span><span class="sxs-lookup"><span data-stu-id="97253-109">Ensure that you have 2 keys created with your Directory ID and onmicrosoft domain.</span></span>

<span data-ttu-id="97253-110">**Configurare l'impostazione del Registro di sistema sul lato client per SCP**</span><span class="sxs-lookup"><span data-stu-id="97253-110">**Configure client-side registry setting for SCP**</span></span>

<span data-ttu-id="97253-111">Usare l'esempio seguente per creare un oggetto Criteri di gruppo per distribuire un'impostazione del Registro di sistema che configura una voce SCP nel Registro di sistema dei dispositivi.</span><span class="sxs-lookup"><span data-stu-id="97253-111">Use the following example to create a Group Policy Object (GPO) to deploy a registry setting that configures an SCP entry in the registry of your devices.</span></span>

1. <span data-ttu-id="97253-112">Aprire una console Gestione Criteri di gruppo e creare un nuovo oggetto Criteri di gruppo nel dominio.</span><span class="sxs-lookup"><span data-stu-id="97253-112">Open a Group Policy Management console and create a new GPO in your domain.</span></span>
     - <span data-ttu-id="97253-113">Specificare un nome per l'oggetto Criteri di gruppo appena creato, ad esempio ClientSideSCP</span><span class="sxs-lookup"><span data-stu-id="97253-113">Provide your newly created GPO a name (for example, ClientSideSCP)</span></span>

2. <span data-ttu-id="97253-114">Modificare l'oggetto Criteri di gruppo e individuare il percorso seguente: **Configurazione computer > Preferenze > Impostazioni di Windows > Registro di sistema**.</span><span class="sxs-lookup"><span data-stu-id="97253-114">Edit the GPO and locate the following path: **Computer Configuration > Preferences > Windows Settings > Registry**.</span></span>

3. <span data-ttu-id="97253-115">Fare clic con il pulsante destro del mouse su **Registro di sistema** e selezionare **Nuovo > Elemento Registro di sistema**.</span><span class="sxs-lookup"><span data-stu-id="97253-115">Right-click on **Registry** and select **New > Registry Item**.</span></span>

4. <span data-ttu-id="97253-116">Nella scheda **Generale** configurare gli elementi seguenti:</span><span class="sxs-lookup"><span data-stu-id="97253-116">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="97253-117">**Azione**: Aggiorna</span><span class="sxs-lookup"><span data-stu-id="97253-117">**Action**: Update</span></span>
    
- <span data-ttu-id="97253-118">**Hive**: HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="97253-118">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="97253-119">**Percorso chiave**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span><span class="sxs-lookup"><span data-stu-id="97253-119">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="97253-120">**Nome valore**: TenantId</span><span class="sxs-lookup"><span data-stu-id="97253-120">**Value name**: TenantId</span></span>
    
- <span data-ttu-id="97253-121">**Tipo di valore**: REG_SZ</span><span class="sxs-lookup"><span data-stu-id="97253-121">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="97253-122">**Dati valore**: GUID o ID directory dell'istanza di Azure AD. Questo valore si trova nel **portale di Azure > Azure Active Directory > Proprietà > ID directory**</span><span class="sxs-lookup"><span data-stu-id="97253-122">**Value data**: The GUID or Directory ID of your Azure AD instance (This value can be found in **Azure portal > Azure Active Directory > Properties > Directory ID**)</span></span>
 
- <span data-ttu-id="97253-123">Fare clic su **OK**.</span><span class="sxs-lookup"><span data-stu-id="97253-123">Click **OK**.</span></span>
 
5. <span data-ttu-id="97253-124">Fare clic con il pulsante destro del mouse su **Registro di sistema** e selezionare **Nuovo > Elemento Registro di sistema**.</span><span class="sxs-lookup"><span data-stu-id="97253-124">Right-click on **Registry** and select **New > Registry Item**.</span></span>

6. <span data-ttu-id="97253-125">Nella scheda **Generale** configurare gli elementi seguenti:</span><span class="sxs-lookup"><span data-stu-id="97253-125">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="97253-126">**Azione**: Aggiorna</span><span class="sxs-lookup"><span data-stu-id="97253-126">**Action**: Update</span></span>
    
- <span data-ttu-id="97253-127">**Hive**: HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="97253-127">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="97253-128">**Percorso chiave**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span><span class="sxs-lookup"><span data-stu-id="97253-128">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="97253-129">**Nome valore**: TenantName</span><span class="sxs-lookup"><span data-stu-id="97253-129">**Value name**: TenantName</span></span>
    
- <span data-ttu-id="97253-130">**Tipo di valore**: REG_SZ</span><span class="sxs-lookup"><span data-stu-id="97253-130">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="97253-131">**Dati valore**: nome di dominio verificato se si usa un ambiente federato, ad esempio AD FS.</span><span class="sxs-lookup"><span data-stu-id="97253-131">**Value data**: Your verified domain name if you are using federated environment such as AD FS.</span></span> <span data-ttu-id="97253-132">Nome di dominio verificato o nome di dominio onmicrosoft.com, ad esempio contoso.onmicrosoft.com, se si usa un ambiente gestito</span><span class="sxs-lookup"><span data-stu-id="97253-132">Your verified domain name or your onmicrosoft.com domain name (for example, contoso.onmicrosoft).com if you are using managed environment</span></span>

- <span data-ttu-id="97253-133">Fare clic su **OK**.</span><span class="sxs-lookup"><span data-stu-id="97253-133">Click **OK**.</span></span>

7. <span data-ttu-id="97253-134">Chiudere l'editor per l'oggetto Criteri di gruppo appena creato.</span><span class="sxs-lookup"><span data-stu-id="97253-134">Close the editor for the newly created GPO.</span></span>

8. <span data-ttu-id="97253-135">Collegare l'oggetto Criteri di gruppo appena creato all'unità organizzativa desiderata contenente i computer aggiunti a un dominio che appartengono alla popolazione di implementazione controllata.</span><span class="sxs-lookup"><span data-stu-id="97253-135">Link the newly created GPO to the desired OU containing domain-joined computers that belong to your controlled rollout population.</span></span>

<span data-ttu-id="97253-136">Per altre informazioni, vedere [Convalida controllata di Aggiunta ad Azure AD ibrido - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) e [Risoluzione dei problemi dei dispositivi ibridi aggiunti ad Azure Active Directory | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span><span class="sxs-lookup"><span data-stu-id="97253-136">For more information, see [Controlled validation of hybrid Azure AD join - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) and  [Troubleshooting hybrid Azure Active Directory joined devices | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span></span>









