---
title: Il writeback delle password non funziona
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
- "9004595"
- "8210"
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 02/12/2021
ms.locfileid: "50232721"
---
# <a name="password-writeback-is-not-working"></a><span data-ttu-id="a6826-102">Il writeback delle password non funziona</span><span class="sxs-lookup"><span data-stu-id="a6826-102">Password Writeback is not working</span></span>

<span data-ttu-id="a6826-103">**Si verificano problemi durante la configurazione del writeback delle password**</span><span class="sxs-lookup"><span data-stu-id="a6826-103">**I'm having problems configuring password writeback**</span></span>

- <span data-ttu-id="a6826-104">Il writeback delle password è una funzionalità premium.</span><span class="sxs-lookup"><span data-stu-id="a6826-104">Password writeback is a premium feature.</span></span>
- <span data-ttu-id="a6826-105">Assicurarsi di comprendere i requisiti di licenza:</span><span class="sxs-lookup"><span data-stu-id="a6826-105">Make sure that you understand the licensing requirements:</span></span>
  - <span data-ttu-id="a6826-106">È necessario disporre di almeno una licenza assegnata nell'organizzazione</span><span class="sxs-lookup"><span data-stu-id="a6826-106">You must have at least one license assigned in your organization</span></span>
  - <span data-ttu-id="a6826-107">**Utenti solo cloud** - Qualsiasi SKU a pagamento di Office 365 (O365) o Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="a6826-107">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
  - <span data-ttu-id="a6826-108">**Utenti cloud e/o** locali : Azure AD Premium P1 o P2, Enterprise Mobility + Security (EMS) o Secure Productive Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="a6826-108">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="a6826-109">Per altre informazioni sui requisiti di licenza, vedere [Requisiti di licenza per la reimpostazione della password in modalità self-service di Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span><span class="sxs-lookup"><span data-stu-id="a6826-109">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span></span>
- <span data-ttu-id="a6826-110">Si dispone di almeno un account amministratore e di un account utente di test con una della licenza appropriata.</span><span class="sxs-lookup"><span data-stu-id="a6826-110">You have at least one administrator account and one test user account with one of the appropriate license.</span></span>
- <span data-ttu-id="a6826-111">Per il funzionamento del writeback delle password, devi connettere Azure AD Connect all'emulatore del controller di dominio primario.</span><span class="sxs-lookup"><span data-stu-id="a6826-111">You must connect Azure AD Connect to the Primary Domain Controller Emulator for password writeback to work.</span></span> <span data-ttu-id="a6826-112">È possibile configurare Azure AD Connect per l'utilizzo  di un controller di dominio primario facendo clic con il pulsante destro del mouse sulle proprietà del connettore di sincronizzazione di Active Directory, quindi selezionando **Configura partizioni di directory.**</span><span class="sxs-lookup"><span data-stu-id="a6826-112">You can configure Azure AD Connect to use a Primary Domain Controller by right clicking on the **properties** of the Active Directory synchronization connector, then selecting **configure directory partitions**.</span></span> <span data-ttu-id="a6826-113">Da qui, cercare la sezione relativa alle impostazioni di connessione **del controller** di dominio e selezionare la casella intitolato Utilizzare solo i controller di **dominio preferiti.**</span><span class="sxs-lookup"><span data-stu-id="a6826-113">From there, look for the **domain controller connection settings** section and check the box titled **only use preferred domain controllers**.</span></span>
  > [!NOTE]
  > <span data-ttu-id="a6826-114">Se il controller di dominio preferito non è un emulatore PDC, Azure AD Connect continuerà a contattare il PDC per il writeback delle password.</span><span class="sxs-lookup"><span data-stu-id="a6826-114">If the preferred DC is not a PDC emulator, Azure AD Connect will still reach out to the PDC for password writeback.</span></span>
- <span data-ttu-id="a6826-115">La reimpostazione della password è stata configurata e abilitata nel tenant.</span><span class="sxs-lookup"><span data-stu-id="a6826-115">Password reset has been configured and enabled in your tenant.</span></span> <span data-ttu-id="a6826-116">Per altre informazioni, vedere Consentire [agli utenti di reimpostare le password di Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)</span><span class="sxs-lookup"><span data-stu-id="a6826-116">For more information, see [Enable users to reset their Azure AD passwords](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).</span></span>
- <span data-ttu-id="a6826-117">Assicurarsi che l'account amministratore utilizzato per abilitare il writeback delle password sia un account amministratore cloud (creato in Azure AD non locale ad)</span><span class="sxs-lookup"><span data-stu-id="a6826-117">Make sure that the administrator account being used to enable Password Writeback is a cloud administrator account (created in Azure AD not on-premises AD)</span></span>
- <span data-ttu-id="a6826-118">Si dispone di una distribuzione locale di Active Directory a foresta singola o a più foreste che esegue Windows Server 2008 R2, Windows Server 2012 o Windows Server 2012 R2 con i Service Pack più recenti installati</span><span class="sxs-lookup"><span data-stu-id="a6826-118">You have a single or multi-forest AD on-premises deployment running Windows Server 2008 R2, Windows Server 2012, or Windows Server 2012 R2 with the latest service packs installed</span></span>
- <span data-ttu-id="a6826-119">Hai installato lo strumento Azure AD Connect e hai preparato l'ambiente AD per la sincronizzazione con il cloud.</span><span class="sxs-lookup"><span data-stu-id="a6826-119">You have the Azure AD Connect tool installed and you have prepared your AD environment for synchronization to the cloud.</span></span> <span data-ttu-id="a6826-120">Prima di testare il writeback delle password, assicurati di completare un'importazione completa e una sincronizzazione completa da AD e Azure AD in Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="a6826-120">Before testing password writeback, make sure that you first complete a full import and full sync from both AD and Azure AD in Azure AD Connect.</span></span>
- <span data-ttu-id="a6826-121">Per altre informazioni, vedere come eseguire una sincronizzazione completa e [l'importazione completa in Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span><span class="sxs-lookup"><span data-stu-id="a6826-121">To learn more, see how to do a [full sync and full import in Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span></span>

<span data-ttu-id="a6826-122">**Si è verificato un problema con la connettività per il writeback delle password**</span><span class="sxs-lookup"><span data-stu-id="a6826-122">**I'm having a problem with password writeback connectivity**</span></span>

1. <span data-ttu-id="a6826-123">Scaricare e abilitare la versione più recente di [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)</span><span class="sxs-lookup"><span data-stu-id="a6826-123">Download and enable the latest version of [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)</span></span>
2. <span data-ttu-id="a6826-124">Configurazione firewall: lo strumento Azure AD Connect (1.1.443 e successive) avrà bisogno dell'accesso **HTTPS** in uscita a:</span><span class="sxs-lookup"><span data-stu-id="a6826-124">Firewall configuration: The Azure AD Connect tool (1.1.443 and above) will need **outbound HTTPS** access to:</span></span>
    - <span data-ttu-id="a6826-125">passwordreset.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="a6826-125">passwordreset.microsoftonline.com</span></span>
    - <span data-ttu-id="a6826-126">servicebus.windows.networks</span><span class="sxs-lookup"><span data-stu-id="a6826-126">servicebus.windows.networks</span></span>
3. <span data-ttu-id="a6826-127">Consenti la persistenza delle connessioni inattive per almeno 2-3 minuti</span><span class="sxs-lookup"><span data-stu-id="a6826-127">Allow idle connections to persist for at least 2-3 minutes</span></span>

<span data-ttu-id="a6826-128">**I'm still having problems with password writeback**</span><span class="sxs-lookup"><span data-stu-id="a6826-128">**I'm still having problems with password writeback**</span></span>

- <span data-ttu-id="a6826-129">Se si hanno ancora difficoltà, provare a disabilitare e abilitare di nuovo il servizio di writeback delle password nello strumento Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="a6826-129">If you are still having difficulty, try disabling and re-enabling the password writeback service in the Azure AD Connect tool</span></span>
- <span data-ttu-id="a6826-130">Per altre informazioni, vedere come disabilitare e [abilitare di nuovo il writeback delle password](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span><span class="sxs-lookup"><span data-stu-id="a6826-130">To learn more, see how to [disable and re-enable password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span></span>
