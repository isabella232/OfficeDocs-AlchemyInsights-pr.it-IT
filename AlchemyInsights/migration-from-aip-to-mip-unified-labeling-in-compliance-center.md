---
title: Migrazione da AIP a MIP/Etichettatura unificata nel Centro conformità
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 7157eada10db2443f64fb7925f408359275d75eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47674330"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="f8889-102">Migrazione da AIP a MIP/Etichettatura unificata nel Centro conformità</span><span class="sxs-lookup"><span data-stu-id="f8889-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="f8889-103">Per passare dalle etichette AIP all'etichettatura unificata nel Centro sicurezza e conformità, procedere come segue:</span><span class="sxs-lookup"><span data-stu-id="f8889-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="f8889-104">**Attivare la protezione nel portale Azure**</span><span class="sxs-lookup"><span data-stu-id="f8889-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="f8889-105">Se non si è già fatto, aprire una nuova finestra del browser e [accedere al portale Azure](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="f8889-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="f8889-106">Passare al pannello **Azure Information Protection**.</span><span class="sxs-lookup"><span data-stu-id="f8889-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="f8889-107">Ad esempio, nel menu Hub, fare clic su **Tutti i servizi** e iniziare a digitare **Informazioni** nella casella Filtro.</span><span class="sxs-lookup"><span data-stu-id="f8889-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="f8889-108">Selezionare **Azure Information Protection**.</span><span class="sxs-lookup"><span data-stu-id="f8889-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="f8889-109">Se non è mai stato effettuato l'accesso al pannello Azure Information Protection prima, consultare i [passaggi aggiuntivi](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) una tantum per aggiungere il pannello al portale.</span><span class="sxs-lookup"><span data-stu-id="f8889-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="f8889-110">Per aprire il pannello Azure Information Protection, bisogna avere un [piano Azure Information Protection Premium](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) o un piano Office 365 che includa Rights Management.</span><span class="sxs-lookup"><span data-stu-id="f8889-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="f8889-111">Se si dispone di uno di questi abbonamenti, ma si visualizza un messaggio che dice che non è possibile trovare un abbonamento valido, [contattare il Supporto tecnico Microsoft](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) o usare i canali di supporto standard.</span><span class="sxs-lookup"><span data-stu-id="f8889-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="f8889-112">Localizzare le opzioni del menu **Gestisci** e selezionare **Attivazione della protezione**.</span><span class="sxs-lookup"><span data-stu-id="f8889-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="f8889-113">Fare clic su **Attiva**, quindi confermare l'operazione.</span><span class="sxs-lookup"><span data-stu-id="f8889-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="f8889-114">Quando l'attivazione è completata, la Barra informazioni mostrerà **L'attivazione è stata completata**.</span><span class="sxs-lookup"><span data-stu-id="f8889-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="f8889-115">**Migrare le etichette di Azure Information Protection al Centro sicurezza e conformità di Office 365**</span><span class="sxs-lookup"><span data-stu-id="f8889-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="f8889-116">Assicurarsi di aver effettuato l'accesso come utente con autorizzazione da amministratore globale.</span><span class="sxs-lookup"><span data-stu-id="f8889-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="f8889-117">Passare al pannello **Azure Information Protection**.</span><span class="sxs-lookup"><span data-stu-id="f8889-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="f8889-118">Nell'opzione del menu **Gestisci** selezionare **Etichettatura unificata**.</span><span class="sxs-lookup"><span data-stu-id="f8889-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="f8889-119">Nel pannello **Azure Information Protection - Etichettatura unificata** fare clic su **Attiva** e seguire le istruzioni online.</span><span class="sxs-lookup"><span data-stu-id="f8889-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="f8889-120">**Nota**: verificare di disporre delle autorizzazioni appropriate prima di attivare la migrazione al Centro sicurezza e conformità.</span><span class="sxs-lookup"><span data-stu-id="f8889-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="f8889-121">Per altre informazioni, vedere questi articoli:</span><span class="sxs-lookup"><span data-stu-id="f8889-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="f8889-122">È necessario essere un amministratore globale per configurare Azure Information Protection o è possibile delegare l'operazione ad altri amministratori?</span><span class="sxs-lookup"><span data-stu-id="f8889-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="f8889-123">Informazioni importanti sui ruoli amministrativi dopo la migrazione al Centro sicurezza e conformità.</span><span class="sxs-lookup"><span data-stu-id="f8889-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="f8889-124">Per altre informazioni sulla migrazione da AIP all'Etichettatura unificata nel Centro sicurezza e conformità, consultare [Migrare le etichette](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span><span class="sxs-lookup"><span data-stu-id="f8889-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
