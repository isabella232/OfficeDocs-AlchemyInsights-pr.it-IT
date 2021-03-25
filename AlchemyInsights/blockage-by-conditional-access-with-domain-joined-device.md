---
title: L'accesso condizionale con un dispositivo aggiunto a un dominio viene bloccato
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: 052311ffe71bcb65de2b5c2a964932b1fb99c373
ms.sourcegitcommit: c34ba92e19419dcb2d251b8a1afe4d180a939617
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 03/20/2021
ms.locfileid: "50965465"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a><span data-ttu-id="dcaea-102">L'accesso condizionale con un dispositivo aggiunto a un dominio viene bloccato</span><span class="sxs-lookup"><span data-stu-id="dcaea-102">I’m getting blocked by Conditional Access with domain joined device</span></span>

<span data-ttu-id="dcaea-103">**Strumenti altamente consigliati**</span><span class="sxs-lookup"><span data-stu-id="dcaea-103">**Highly Recommended Tools**</span></span>

<span data-ttu-id="dcaea-104">[Strumento di risoluzione dei problemi di registrazione dei dispositivi](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/): lo strumento che consente di risolvere i problemi di registrazione dei dispositivi più comuni.</span><span class="sxs-lookup"><span data-stu-id="dcaea-104">[Device Registration Troubleshooter Tool](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - The tool that helps in troubleshooting the most common device registration issues.</span></span>

<span data-ttu-id="dcaea-105">[Script di test della connettività per la registrazione dei dispositivi](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/): lo script che consente di verificare che un dispositivo possa accedere agli endpoint di registrazione dei dispositivi nell'account di sistema.</span><span class="sxs-lookup"><span data-stu-id="dcaea-105">[Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - The script that helps ensuring that a device can access Device Registration endpoints under the system account.</span></span>

<span data-ttu-id="dcaea-106">[Script di pulizia dei dispositivi Azure AD](https://github.com/mzmaili/AzureADDeviceCleanup): lo script che consente di cercare e gestire dispositivi obsoleti nell'ambiente.</span><span class="sxs-lookup"><span data-stu-id="dcaea-106">[Azure AD Device Cleanup Script](https://github.com/mzmaili/AzureADDeviceCleanup) - The script that enables you to seek and manage stale devices in your environment.</span></span>

<span data-ttu-id="dcaea-107">Ecco alcuni motivi comuni per cui l'accesso condizionale potrebbe non riuscire in un dispositivo aggiunto a un dominio (Azure AD ibrido).</span><span class="sxs-lookup"><span data-stu-id="dcaea-107">Here are some common reasons why conditional access may be failing a device that has joined a domain (Hybrid Azure AD).</span></span>

1. <span data-ttu-id="dcaea-108">**Non è presente un PRT di Azure AD nel dispositivo**: è necessario verificare che il dispositivo disponga di un token di aggiornamento primario (PRT) di Azure AD.</span><span class="sxs-lookup"><span data-stu-id="dcaea-108">**There’s no Azure AD PRT on the device** - You need to ensure that the device has Azure AD Primary Refresh Token (PRT).</span></span> <span data-ttu-id="dcaea-109">Per altre informazioni sul PRT, consultare questo [documento](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span><span class="sxs-lookup"><span data-stu-id="dcaea-109">For more information about PRT, see this [document](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="dcaea-110">Per verificare la presenza di un PRT di Azure AD, è possibile eseguire il comando `dsregcmd/status` nel dispositivo e verificare se "AzureAdPrt" è uguale a "YES".</span><span class="sxs-lookup"><span data-stu-id="dcaea-110">To verify if you have Azure AD PRT, you can run `dsregcmd/status` command on the device and verify if “AzureAdPrt” equals “YES”.</span></span>

<span data-ttu-id="dcaea-111">Se "AzureAdPrt" è "NO", verificare quanto segue:</span><span class="sxs-lookup"><span data-stu-id="dcaea-111">If "AzureAdPrt" is "NO", check the following:</span></span>

- <span data-ttu-id="dcaea-112">**Se è presente un ambiente federato con AD FS e non è raggiungibile dalle reti domestiche degli utenti**: in questo caso, verificare che gli endpoint "usernamemixed" siano accessibili dalla Extranet.</span><span class="sxs-lookup"><span data-stu-id="dcaea-112">**Whether you have a federated environment with AD FS, and it’s unreachable from your users’ home networks**: In this case, ensure that your "usernamemixed" endpoints are accessible from the extranet.</span></span> <span data-ttu-id="dcaea-113">Se AD FS è dietro una VPN, verificare che gli utenti siano connessi alla VPN e accedere di nuovo al dispositivo.</span><span class="sxs-lookup"><span data-stu-id="dcaea-113">If your AD FS is behind a VPN, ensure that the users connect to the VPN and re-login to the device.</span></span> <span data-ttu-id="dcaea-114">Per altre informazioni, consultare questo [documento](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).</span><span class="sxs-lookup"><span data-stu-id="dcaea-114">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).</span></span>

- <span data-ttu-id="dcaea-115">**Se il TPM del dispositivo è difettoso e non è possibile autenticare il dispositivo**: controllare "tpm.msc" per vedere se lo stato del TPM è "Ready".</span><span class="sxs-lookup"><span data-stu-id="dcaea-115">**Whether the device’s TPM is faulty and thus cannot authenticate the device**: Check "tpm.msc" to see if the state of TPM is "Ready".</span></span> <span data-ttu-id="dcaea-116">In caso contrario, eseguire `dsregcmd/leave` e consentire al dispositivo di aggiungersi di nuovo ad Azure AD.</span><span class="sxs-lookup"><span data-stu-id="dcaea-116">If not, run `dsregcmd/leave` and let the device re-join to Azure AD.</span></span> <span data-ttu-id="dcaea-117">Quindi riprovare.</span><span class="sxs-lookup"><span data-stu-id="dcaea-117">Then, try again.</span></span> <span data-ttu-id="dcaea-118">Per altre informazioni, consultare questo [documento](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span><span class="sxs-lookup"><span data-stu-id="dcaea-118">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>

- <span data-ttu-id="dcaea-119">**È in uso un provider di identità di terze parti che non supporta il protocollo WS-Trust**.</span><span class="sxs-lookup"><span data-stu-id="dcaea-119">**You’re using a 3rd party identity provider, which does not support WS-Trust protocol**.</span></span> <span data-ttu-id="dcaea-120">Come descritto nei documenti, i dispositivi aggiunti ad Azure AD ibrido non possono funzionare in questo caso.</span><span class="sxs-lookup"><span data-stu-id="dcaea-120">As described in our docs, hybrid Azure AD-joined devices cannot work in this case.</span></span> <span data-ttu-id="dcaea-121">Contattare il provider di identità per ricevere assistenza.</span><span class="sxs-lookup"><span data-stu-id="dcaea-121">Please work with your Identity provider for support.</span></span>

2. <span data-ttu-id="dcaea-122">**Gli utenti usano il browser Chrome senza account di Windows 10** oppure l'**estensione Office per Chrome non usa automaticamente il PRT nei dispositivi aggiunti ad AAD o ad AAD ibrido**: questo causa l'errore dei criteri di accesso condizionale basati su dispositivo, con il messaggio di errore "Dispositivo non registrato" visualizzato.</span><span class="sxs-lookup"><span data-stu-id="dcaea-122">**Users are using Chrome browser without the Windows 10 Accounts** or **Office extension Chrome does not automatically use the PRT on AAD-joined or hybrid-AAD-joined devices**: This leads to failure of any device-based Conditional Access policies, with “Unregistered device” error message displayed.</span></span> <span data-ttu-id="dcaea-123">Per usare correttamente il browser Chrome, è necessario installare "Account Windows 10" o l'"estensione di Office per il browser Chrome degli utenti" tramite SCCM o Intune.</span><span class="sxs-lookup"><span data-stu-id="dcaea-123">To use Chrome browser correctly, you must install the “Windows 10 Accounts” or "Office extension to the users’ Chrome browser" via SCCM or Intune.</span></span> <span data-ttu-id="dcaea-124">Per altre informazioni, consultare questo [documento](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span><span class="sxs-lookup"><span data-stu-id="dcaea-124">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span></span>

<span data-ttu-id="dcaea-125">Se non è possibile eseguire il push dell'estensione da remoto, avvisare gli utenti di installare manualmente una delle estensioni precedenti per accedere alle applicazioni dietro l'accesso condizionale basato su dispositivo.</span><span class="sxs-lookup"><span data-stu-id="dcaea-125">If it’s not possible to push the extension remotely, notify users to manually install one of the above extensions to access applications behind device-based Conditional Access.</span></span> <span data-ttu-id="dcaea-126">Per altre informazioni, consultare questo [documento](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).</span><span class="sxs-lookup"><span data-stu-id="dcaea-126">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).</span></span>

3. <span data-ttu-id="dcaea-127">**Il dispositivo è stato aggiunto ad Azure AD ibrido correttamente ma è stato eliminato o disabilitato inavvertitamente, a causa di modifiche alla sincronizzazione in Azure AD Connect o del portale di Azure**: in questo caso, l'oggetto del dispositivo non è più riconosciuto come dispositivo aggiunto anche se lo stato di "AzureAdJoined" e "PRT" risulta valido nel dispositivo.</span><span class="sxs-lookup"><span data-stu-id="dcaea-127">**The device was correctly hybrid Azure AD joined, but it was inadvertently deleted or disabled, either due to sync changes in Azure AD Connect or from the Azure portal**: If this happens, the device object is no longer recognized as a fully joined device even though the "AzureAdJoined" and "PRT" status show up as valid on the device.</span></span>

<span data-ttu-id="dcaea-128">Per risolvere il problema, eseguire `dsregcmd/leave` nei dispositivi interessati e consentire loro di aggiungersi di nuovo ad Azure AD.</span><span class="sxs-lookup"><span data-stu-id="dcaea-128">To fix this issue, run `dsregcmd/leave` on the affected devices and let them rejoin Azure AD.</span></span> <span data-ttu-id="dcaea-129">Per altre informazioni, consultare questo [documento](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).</span><span class="sxs-lookup"><span data-stu-id="dcaea-129">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).</span></span>

> [!NOTE]
> <span data-ttu-id="dcaea-130">Se i dispositivi sono in esecuzione con l'aggiornamento 1809 di Windows 10, con proxy VPN/Cloud e si verificano problemi con lo stato di "AzureAdPrt" o con un'app con problemi di SSO (Outlook non si connette alla cassetta postale anche se è presente un PRT), verificare di disporre della patch [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) o dell'aggiornamento cumulativo di aprile [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) per evitare errori di PRT in tali computer.</span><span class="sxs-lookup"><span data-stu-id="dcaea-130">If your devices are on Windows 10, 1809 update, with VPN/Cloud Proxy and see issues with "AzureAdPrt" state or any app with SSO problem (outlook not connecting to mailbox even though you had PRT), ensure you have this patch [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) or April cumulative update [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) to prevent PRT failures on those machines.</span></span>

















