---
title: Problemi di gestione utenti
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9209"
- "9005371"
ms.openlocfilehash: 4b61686381de0cafa38857ca7a96b3a81aa191ec
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 03/19/2021
ms.locfileid: "50898163"
---
# <a name="user-management-issues"></a><span data-ttu-id="07387-102">Problemi di gestione utenti</span><span class="sxs-lookup"><span data-stu-id="07387-102">User management issues</span></span>

<span data-ttu-id="07387-103">**Cosa succede agli utenti attualmente assegnati all’applicazione se viene disabilitata la proprietà ‘Assegnazione utenti obbligatoria’ (proprietà impostata su No)?**</span><span class="sxs-lookup"><span data-stu-id="07387-103">**What happens to current assigned users to the application if I disable the property ‘User assignment required’ (set this property to No)?**</span></span>

<span data-ttu-id="07387-104">La disattivazione della **Assegnazione utenti obbligatoria** NON influisce sugli utenti attualmente assegnati.</span><span class="sxs-lookup"><span data-stu-id="07387-104">Disabling **User assignment required** does NOT affect the currently assigned users.</span></span> <span data-ttu-id="07387-105">La disattivazione di questa proprietà consentirà a tutti gli utenti di accedere all’applicazione. </span><span class="sxs-lookup"><span data-stu-id="07387-105">Disabling this property will only allow all users to access the application.</span></span> <span data-ttu-id="07387-106">Tutti gli utenti elencati e gli utenti assegnati a gruppi nell’applicazione continueranno ad essere validi.</span><span class="sxs-lookup"><span data-stu-id="07387-106">All the listed users and those users assigned to groups in the application will still be valid.</span></span>

- <span data-ttu-id="07387-107">Per limitare l’app a uno specifico gruppo di utenti, vedere [Limitare l’app Azure AD a un gruppo di utenti - Microsoft Identity Platform | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.).</span><span class="sxs-lookup"><span data-stu-id="07387-107">To restrict your app to specific set of users, see - [Restrict Azure AD app to a set of users - Microsoft identity platform | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.).</span></span>
- <span data-ttu-id="07387-108">Per l’assegnazione di utenti e gruppi ad applicazioni aziendali in Azure Active Directory (Azure AD), dal portale di Azure o utilizzando PowerShell, vedere [Gestire l’assegnazione di utenti ad una app in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal).</span><span class="sxs-lookup"><span data-stu-id="07387-108">To assign users and groups, to enterprise applications in Azure Active Directory (Azure AD), either from within the Azure portal or by using PowerShell, see [Manage user assignment for an app in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal).</span></span>
- <span data-ttu-id="07387-109">Per delegare le autorizzazioni per la creazione e la gestione di applicazioni, vedere [Delegare le autorizzazioni di amministratore per la gestione di applicazioni - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles).</span><span class="sxs-lookup"><span data-stu-id="07387-109">To delegate Application creation and management permissions, see [Delegate application management administrator permissions - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles).</span></span>
- <span data-ttu-id="07387-110">**Nascondere specifiche app aziendali agli utenti** - Eseguire i seguenti passaggi per nascondere tutte le app di Microsoft 365 dal pannello **App personali**.</span><span class="sxs-lookup"><span data-stu-id="07387-110">**Hide specific enterprise apps from users** - Use the following steps to hide all Microsoft 365 apps from the **MyApps** panel.</span></span> <span data-ttu-id="07387-111">Le app saranno ancora visibili nel portale di Office 365.</span><span class="sxs-lookup"><span data-stu-id="07387-111">The apps will still be visible in the Office 365 portal.</span></span>

 1. <span data-ttu-id="07387-112">Accedere al portale di Azure come amministratore globale della directory.</span><span class="sxs-lookup"><span data-stu-id="07387-112">Sign-in to the Azure portal as a global administrator for your directory.</span></span> 
 2. <span data-ttu-id="07387-113">Selezionare **Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="07387-113">Select **Azure Active Directory**.</span></span> 
 3. <span data-ttu-id="07387-114">Selezionare **Utenti**.</span><span class="sxs-lookup"><span data-stu-id="07387-114">Select **Users**.</span></span> 
 4. <span data-ttu-id="07387-115">Selezionare **Impostazioni utente**.</span><span class="sxs-lookup"><span data-stu-id="07387-115">Select **User settings**.</span></span> 
 5. <span data-ttu-id="07387-116">In **Applicazioni aziendali**, fare clic su **Gestire come gli utenti finali avviano e visualizzano le applicazioni**.</span><span class="sxs-lookup"><span data-stu-id="07387-116">Under **Enterprise applications**, click **Manage how end users launch and view their applications**.</span></span> 
 6. <span data-ttu-id="07387-117">Per **Gli utenti possono vedere solo le app di Office 365 nel portale di Office 365**, fare clic su **Sì**.</span><span class="sxs-lookup"><span data-stu-id="07387-117">For **Users can only see Office 365 apps in the Office 365 portal**, click **Yes**.</span></span> 
 7. <span data-ttu-id="07387-118">Fare clic su **Salva**.</span><span class="sxs-lookup"><span data-stu-id="07387-118">Click **Save**.</span></span> 
 8. <span data-ttu-id="07387-119">Per altri dettagli, vedere [Nascondere un’applicazione aziendale dall’esperienza dell’utente in Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)</span><span class="sxs-lookup"><span data-stu-id="07387-119">For more details, see [Hide an Enterprise application from user's experience in Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)</span></span>

- <span data-ttu-id="07387-120">Se si offre una applicazione SaaS (Software come servizio) a diverse organizzazioni, è possibile configurare l’app in modo che accetti gli accessi da qualsiasi tenant Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="07387-120">If you offer a Software as a Service (SaaS) app to many organizations, you can configure your app to accept sign-ins from any Azure Active Directory (Azure AD) tenant.</span></span> <span data-ttu-id="07387-121">Questa configurazione è chiamata "applicazione multi-tenant".</span><span class="sxs-lookup"><span data-stu-id="07387-121">This configuration is called "making your application multi-tenant".</span></span> <span data-ttu-id="07387-122">Gli utenti in qualsiasi tenant Azure AD potranno accedere all’app dopo aver acconsentito a utilizzare il proprio account nell’app.</span><span class="sxs-lookup"><span data-stu-id="07387-122">Users in any Azure AD tenant will be able to sign-in to your app after consenting to use their account with your app.</span></span> <span data-ttu-id="07387-123">Per altre informazioni, vedere [Creare app che consentono l’accesso ad utenti Azure AD - Microsoft Identity Platform | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant).</span><span class="sxs-lookup"><span data-stu-id="07387-123">For more information, see [Build apps that sign in Azure AD users - Microsoft identity platform | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant).</span></span>

- <span data-ttu-id="07387-124">**In che modo un utente finale può accedere all’applicazione una volta che è stato assegnato all’applicazione?**</span><span class="sxs-lookup"><span data-stu-id="07387-124">**How can an end user access the application once he/she is assigned to the application?**</span></span>

<span data-ttu-id="07387-125">Ogni app nel pannello Applicazioni aziendali contiene un collegamento per l’accesso degli utenti finali.</span><span class="sxs-lookup"><span data-stu-id="07387-125">Each app in Enterprise application blade has a link for end users to access.</span></span> <span data-ttu-id="07387-126">Gli utenti possono accedere facilmente all’app anche attraverso il portale **App personali**.</span><span class="sxs-lookup"><span data-stu-id="07387-126">Users can also access the app through **Myapps** portal in an easy way.</span></span>

- <span data-ttu-id="07387-127">**Si vuole sapere quali applicazioni e tipi di applicazioni sono in uso da parte degli utenti?**</span><span class="sxs-lookup"><span data-stu-id="07387-127">**Want to know which applications and type of applications are being used by users?**</span></span>

<span data-ttu-id="07387-128">È possibile scaricare i report degli accessi degli ultimi 30 giorni da **portal.azure.com > Azure Active Directory> Accessi> scarica i report**.</span><span class="sxs-lookup"><span data-stu-id="07387-128">You can download sign-in reports for the last 30 days from **portal.azure.com > Azure Active directory> Signins> download reports**.</span></span>

- <span data-ttu-id="07387-129">Informazioni su come [Concedere al tenant un ampio consenso amministratore per una applicazione](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) e [Configurare come gli utenti finali concedono l’autorizzazione alle applicazioni](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent).</span><span class="sxs-lookup"><span data-stu-id="07387-129">Learn how to [Grant tenant wide admin consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) and [Configure how end users consent to applications](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent).</span></span>

- <span data-ttu-id="07387-130">Informazioni su [come funziona l’autorizzazione](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) e [Gestire l’autorizzazione per le applicazioni](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests).</span><span class="sxs-lookup"><span data-stu-id="07387-130">Understand [how consent works](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) and [Manage consent to applications](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests).</span></span>

