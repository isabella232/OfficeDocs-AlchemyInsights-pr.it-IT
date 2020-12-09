---
title: Abilitare la gestione dei costi
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6463"
ms.openlocfilehash: 0bbf1158f7f5fa8a22cfe7242c86760057fc7bab
ms.sourcegitcommit: 0f26f6b23b3d48c3c6cddf98bc41df484f16cb00
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/08/2020
ms.locfileid: "49599081"
---
# <a name="enable-cost-management"></a><span data-ttu-id="3bb24-102">Abilitare la gestione dei costi</span><span class="sxs-lookup"><span data-stu-id="3bb24-102">Enable cost management</span></span>

<span data-ttu-id="3bb24-103">**Che cosa significa ' i costi sono disattivati per l'organizzazione '?**</span><span class="sxs-lookup"><span data-stu-id="3bb24-103">**What does 'costs are disabled for your organization' mean?**</span></span>

<span data-ttu-id="3bb24-104">Le organizzazioni che utilizzano gli account Enterprise Agreement (EA) o Microsoft Customer Agreement (MCA) possono disabilitare l'accesso alle informazioni sui costi e alle informazioni sui prezzi.</span><span class="sxs-lookup"><span data-stu-id="3bb24-104">Organizations using Enterprise Agreement (EA) or Microsoft Customer Agreement (MCA) accounts can disable access to cost information and pricing information.</span></span>

<span data-ttu-id="3bb24-105">Dopo aver eseguito l'accesso al portale di Azure, è possibile utilizzare le API di fatturazione per ottenere fatture a livello di programmazione (una volta che sono stati scelti) e dettagli sull'utilizzo.</span><span class="sxs-lookup"><span data-stu-id="3bb24-105">After logging in to Azure portal, they can use the Billing APIs to programmatically get invoices (once opted-in) and usage details.</span></span>

<span data-ttu-id="3bb24-106">**Informazioni su come consentire agli utenti aggiuntivi di accedere alle fatture**</span><span class="sxs-lookup"><span data-stu-id="3bb24-106">**How to allow additional users to access invoices**</span></span>

1. <span data-ttu-id="3bb24-107">Andare a **Blade abbonamenti** nel portale di Azure.</span><span class="sxs-lookup"><span data-stu-id="3bb24-107">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="3bb24-108">Selezionare **fatture** e quindi **accedere alle fatture**.</span><span class="sxs-lookup"><span data-stu-id="3bb24-108">Select **Invoices** and then **Access to invoices**.</span></span>
3. <span data-ttu-id="3bb24-109">Attivare l'accesso, seguito salvando le modifiche, per consentire agli utenti di ruoli con ambito sottoscrizione di scaricare le fatture.</span><span class="sxs-lookup"><span data-stu-id="3bb24-109">Turn on the access, followed by saving the changes, to allow users in subscription-scoped roles to download invoices.</span></span>

> [!NOTE]
> <span data-ttu-id="3bb24-110">L'amministratore dell'account può anche configurare la possibilità di inviare fatture tramite posta elettronica.</span><span class="sxs-lookup"><span data-stu-id="3bb24-110">The Account Administrator can also configure to have invoices sent via email.</span></span> <span data-ttu-id="3bb24-111">Per ulteriori informazioni, vedere [ottenere la fattura tramite posta elettronica](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span><span class="sxs-lookup"><span data-stu-id="3bb24-111">To learn more, see [Get your invoice in email](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span></span>

<span data-ttu-id="3bb24-112">**Come aggiungere gli utenti al ruolo del lettore di fatturazione**</span><span class="sxs-lookup"><span data-stu-id="3bb24-112">**How to add users to the Billing Reader role**</span></span>

1. <span data-ttu-id="3bb24-113">Andare a **Blade abbonamenti** nel portale di Azure.</span><span class="sxs-lookup"><span data-stu-id="3bb24-113">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="3bb24-114">Selezionare **controllo di accesso (IAM)** e quindi fare clic su **Aggiungi**.</span><span class="sxs-lookup"><span data-stu-id="3bb24-114">Select **Access control (IAM)** and then click **Add**.</span></span>
3. <span data-ttu-id="3bb24-115">Scegliere **Billing Reader** nella pagina **selezionare un ruolo** .</span><span class="sxs-lookup"><span data-stu-id="3bb24-115">Choose **Billing Reader** in the **Select a role** page.</span></span>
4. <span data-ttu-id="3bb24-116">Digitare il messaggio di posta elettronica dell'utente che si desidera invitare e quindi fare clic su **OK** per inviare l'invito.</span><span class="sxs-lookup"><span data-stu-id="3bb24-116">Type the email of the user you want to invite, and then click **OK** to send the invitation.</span></span>
5. <span data-ttu-id="3bb24-117">Seguire le istruzioni fornite nel messaggio di posta elettronica invita per accedere come lettore di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="3bb24-117">Follow instructions provided in the invite email to log in as a billing reader.</span></span> <span data-ttu-id="3bb24-118">Per ulteriori informazioni, vedere [concedere l'accesso alla fatturazione](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span><span class="sxs-lookup"><span data-stu-id="3bb24-118">For more information, see [Grant access to Billing](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span></span>

<span data-ttu-id="3bb24-119">**Documenti consigliati**</span><span class="sxs-lookup"><span data-stu-id="3bb24-119">**Recommended documents**</span></span>

- [<span data-ttu-id="3bb24-120">Abilitare le visualizzazioni DA e AO tramite il portale EA</span><span class="sxs-lookup"><span data-stu-id="3bb24-120">Enable DA and AO views via EA portal</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [<span data-ttu-id="3bb24-121">Costi inclusi nella gestione dei costi</span><span class="sxs-lookup"><span data-stu-id="3bb24-121">Costs included in Cost Management</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [<span data-ttu-id="3bb24-122">Offerte di Microsoft Azure supportate</span><span class="sxs-lookup"><span data-stu-id="3bb24-122">Supported Microsoft Azure Offers</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [<span data-ttu-id="3bb24-123">Esaminare i costi nell'analisi dei costi</span><span class="sxs-lookup"><span data-stu-id="3bb24-123">Review costs in cost analysis</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [<span data-ttu-id="3bb24-124">Fornire l'accesso alle informazioni di fatturazione</span><span class="sxs-lookup"><span data-stu-id="3bb24-124">Provide access to billing information</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="3bb24-125">Controllare l'accesso a un contratto per i clienti Microsoft</span><span class="sxs-lookup"><span data-stu-id="3bb24-125">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






