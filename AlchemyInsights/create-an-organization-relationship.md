---
title: Creare una relazione organizzativa per consentire agli utenti di collaborare con un'altra organizzazione
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 2c6cd6a178c6e012bfe1c8d769b037168ffa3254
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 06/23/2020
ms.locfileid: "44854014"
---
# <a name="create-an-organization-relationship-to-allow-your-users-to-collaborate-with-another-organization"></a><span data-ttu-id="75af1-102">Creare una relazione organizzativa per consentire agli utenti di collaborare con un'altra organizzazione</span><span class="sxs-lookup"><span data-stu-id="75af1-102">Create an Organization Relationship to allow your users to collaborate with another organization</span></span>

1. <span data-ttu-id="75af1-103">Dal dashboard dell'interfaccia di amministrazione di Microsoft 365, passare a **Amministrazione** > **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="75af1-103">From the Microsoft 365 admin center dashboard, go to **Admin** > **Exchange**.</span></span>
2. <span data-ttu-id="75af1-104">Passare a **organizzazione** > **condivisione**.</span><span class="sxs-lookup"><span data-stu-id="75af1-104">Go to **organization** > **sharing**.</span></span>
3. <span data-ttu-id="75af1-105">In **Condivisione tra organizzazioni** fare clic su **Nuovo** .</span><span class="sxs-lookup"><span data-stu-id="75af1-105">Under **Organization Sharing**, click **New** .</span></span>
4. <span data-ttu-id="75af1-106">In **Nuova relazione organizzativa**, nella casella **Nome relazione**, digitare un nome amico per la relazione organizzativa.</span><span class="sxs-lookup"><span data-stu-id="75af1-106">In **new organization relationship**, in the **Relationship name** box, type a friendly name for the organization relationship.</span></span>
5. <span data-ttu-id="75af1-p101">Nella casella **Domini da condividere con**, digitare il dominio per l'organizzazione federata esterna di Exchange o Office 365 che si desidera configurare per la condivisione federata. Se necessario immettere più di un dominio, separare i nomi dei domini con una virgola. Ad esempio, contoso.com, service.contoso.com.</span><span class="sxs-lookup"><span data-stu-id="75af1-p101">In the **Domains to share with** box, type the domain for the external Office 365 or Exchange on-premises organization you want to let see your calendars. If you need to enter more than one domain, separate the domain names with a comma. For example, contoso.com, service.contoso.com.</span></span>
6. <span data-ttu-id="75af1-p102">Selezionare la casella di controllo **Abilitare la condivisione delle informazioni di disponibilità calendario** per attivare la condivisione del calendario con i domini elencati. Impostare il livello di condivisione delle informazioni sulla disponibilità e impostare quale utente può condividerle.</span><span class="sxs-lookup"><span data-stu-id="75af1-p102">Select the **Enable calendar free/busy information sharing** check box to turn on calendar sharing with the domains you listed. Set the sharing level for calendar free/busy information and set which users can share calendar free/busy information.</span></span>  

<span data-ttu-id="75af1-112">Per impostare il livello di accesso alle informazioni sulla disponibilità, selezionare una delle seguenti operazioni:</span><span class="sxs-lookup"><span data-stu-id="75af1-112">To set the free/busy access level, select one of the following:</span></span>

- <span data-ttu-id="75af1-113">**Informazioni sulla disponibilità in calendario, solo con data/ora**</span><span class="sxs-lookup"><span data-stu-id="75af1-113">**Calendar free/busy information with time only**</span></span>
- <span data-ttu-id="75af1-114">**   Informazioni sulla disponibilità con ora, oggetto e posizione**</span><span class="sxs-lookup"><span data-stu-id="75af1-114">**Calendar free/busy with time, subject, and location**</span></span>  

 <span data-ttu-id="75af1-115">Per impostare quali utenti condivideranno le informazioni sulla disponibilità, selezionare una delle voci seguenti:</span><span class="sxs-lookup"><span data-stu-id="75af1-115">To set which users will share calendar free/busy information, select one of the following:</span></span>

- <span data-ttu-id="75af1-116">**Tutti gli utenti dell'organizzazione**</span><span class="sxs-lookup"><span data-stu-id="75af1-116">**Everyone in your organization**</span></span>
- <span data-ttu-id="75af1-117">**Un gruppo di protezione specificato**</span><span class="sxs-lookup"><span data-stu-id="75af1-117">**A specified security group**</span></span>  

<span data-ttu-id="75af1-118">Fare clic su **Sfoglia** per selezionare il gruppo di sicurezza da un elenco, fare clic su **ok**.</span><span class="sxs-lookup"><span data-stu-id="75af1-118">Click **browse** to pick the security group from a list, then click **ok**.</span></span>

<span data-ttu-id="75af1-119">Fare clic su **Salva** per creare la relazione organizzativa.</span><span class="sxs-lookup"><span data-stu-id="75af1-119">Click **save** to create the organization relationship.</span></span>  

<span data-ttu-id="75af1-120">**Nota:** le configurazioni tra tenant non supportano la ricerca di informazioni sulla disponibilità tra i contatti personali.</span><span class="sxs-lookup"><span data-stu-id="75af1-120">**Note:** Cross-tenant configurations do not support personal contacts for free/busy lookup.</span></span> <span data-ttu-id="75af1-121">I contatti devono essere inclusi nell'elenco indirizzi globale per il funzionamento della la ricerca della disponibilità.</span><span class="sxs-lookup"><span data-stu-id="75af1-121">Contacts must be included in the global address list for free/busy lookup to work.</span></span>

<span data-ttu-id="75af1-122">**Per informazioni complete su questo argomento, vedere:**</span><span class="sxs-lookup"><span data-stu-id="75af1-122">**For full understanding of this topic please read:**</span></span>

- [<span data-ttu-id="75af1-123">Creare una relazione dell'organizzazione in Exchange Online</span><span class="sxs-lookup"><span data-stu-id="75af1-123">Create an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/create-an-organization-relationship)
- [<span data-ttu-id="75af1-124">Modificare una relazione dell'organizzazione in Exchange Online</span><span class="sxs-lookup"><span data-stu-id="75af1-124">Modify an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/modify-an-organization-relationship)
- [<span data-ttu-id="75af1-125">Rimuovere una relazione dell'organizzazione in Exchange Online</span><span class="sxs-lookup"><span data-stu-id="75af1-125">Remove an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/remove-an-organization-relationship)
