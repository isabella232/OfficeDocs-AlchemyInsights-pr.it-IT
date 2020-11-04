---
title: Trasferire la proprietà della fatturazione di Azure
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
- "9003560"
- "6849"
ms.openlocfilehash: e9a1e74b321e2c2dda5f7a4f69681a0acf0635d5
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 11/03/2020
ms.locfileid: "48840608"
---
# <a name="transfer-azure-billing-ownership"></a><span data-ttu-id="38cf1-102">Trasferire la proprietà della fatturazione di Azure</span><span class="sxs-lookup"><span data-stu-id="38cf1-102">Transfer Azure billing ownership</span></span>

<span data-ttu-id="38cf1-103">Accede al [portale di Azure](https://portal.azure.com/) con il ruolo di Amministratore dell'account di fatturazione che include la sottoscrizione che si vuole trasferire.</span><span class="sxs-lookup"><span data-stu-id="38cf1-103">Sign in to the [Azure portal](https://portal.azure.com/) as an administrator of the billing account that has the subscription that you want to transfer.</span></span> <span data-ttu-id="38cf1-104">Se non si è certi di essere amministratori o se è necessario determinare l'amministratore, vedere [Determinare l'amministratore della fatturazione dell'account](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span><span class="sxs-lookup"><span data-stu-id="38cf1-104">If you're not sure if you're and administrator, or if you need to determine who is, see [Determine account billing administrator](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span></span>

- <span data-ttu-id="38cf1-105">Cercare in **Gestione costi e fatturazione**.</span><span class="sxs-lookup"><span data-stu-id="38cf1-105">Search on **Cost Management + Billing**.</span></span>
- <span data-ttu-id="38cf1-106">Selezionare **Sottoscrizioni** nel riquadro sinistro.</span><span class="sxs-lookup"><span data-stu-id="38cf1-106">Select **Subscriptions** from left pane.</span></span> <span data-ttu-id="38cf1-107">A seconda del tipo di accesso, potrebbe essere necessario selezionare un ambito di fatturazione, poi **Sottoscrizioni** o **Sottoscrizioni di Azure**.</span><span class="sxs-lookup"><span data-stu-id="38cf1-107">Depending on the access, you may need to select a billing scope and then **Subscriptions** or **Azure subscriptions**.</span></span>
- <span data-ttu-id="38cf1-108">Selezionare **Trasferisci la proprietà della fatturazione** per la sottoscrizione che si vuole trasferire</span><span class="sxs-lookup"><span data-stu-id="38cf1-108">Select **Transfer billing ownership** for the subscription you want to transfer</span></span>
- <span data-ttu-id="38cf1-109">Immettere l'indirizzo di posta elettronica dell'utente, già amministratore fatturazione dell'account, che diventerà il nuovo proprietario della sottoscrizione, poi selezionare **Invia richiesta di trasferimento**</span><span class="sxs-lookup"><span data-stu-id="38cf1-109">Enter the email address of a user who's a billing administrator of the account that will be the new owner for the subscription and then select **send transfer request**</span></span>
- <span data-ttu-id="38cf1-110">L'utente riceverà un messaggio di posta elettronica con le istruzioni per verificare la richiesta di trasferimento.</span><span class="sxs-lookup"><span data-stu-id="38cf1-110">The user gets an email with instructions to review your transfer request.</span></span> <span data-ttu-id="38cf1-111">Per approvare la richiesta, l'utente deve selezionare il collegamento nel messaggio di posta elettronica e seguire le istruzioni.</span><span class="sxs-lookup"><span data-stu-id="38cf1-111">To approve the transfer request, the user selects the link in the email and follows the instructions.</span></span>

<span data-ttu-id="38cf1-112">**Nota** : se si trasferisce la proprietà della fatturazione relativa alla sottoscrizione a un account utente di un altro tenant di Azure AD, tutte le assegnazioni di [Controllo accessi in base al ruolo (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) per la gestione delle risorse nella sottoscrizione verranno rimosse definitivamente.</span><span class="sxs-lookup"><span data-stu-id="38cf1-112">**Note** : If you transfer billing ownership of your subscription to a user's account in another Azure AD tenant, all [role-based access control (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)assignments to manage resources in the subscription are permanently removed.</span></span> <span data-ttu-id="38cf1-113">Solo il nuovo proprietario avrà accesso alla gestione delle risorse nella sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="38cf1-113">Only the new owner will have access to manage resources in the subscription.</span></span> <span data-ttu-id="38cf1-114">Per altre informazioni, vedere [Trasferimento di una sottoscrizione a un utente di un altro tenant di Azure AD](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="38cf1-114">For more information, see [Transferring subscription to a user in another Azure AD tenant](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="38cf1-115">**Documenti consigliati**</span><span class="sxs-lookup"><span data-stu-id="38cf1-115">**Recommended Documents**</span></span>

- [<span data-ttu-id="38cf1-116">Trasferire la proprietà della fatturazione di una sottoscrizione di Azure a un altro account</span><span class="sxs-lookup"><span data-stu-id="38cf1-116">Transfer billing ownership of an Azure subscription to another account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [<span data-ttu-id="38cf1-117">Informazioni sul trasferimento della proprietà di fatturazione per una sottoscrizione di Azure</span><span class="sxs-lookup"><span data-stu-id="38cf1-117">About transferring billing ownership for an Azure subscription</span></span>](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [<span data-ttu-id="38cf1-118">Trasferimento delle sottoscrizioni di Visual Studio, Microsoft Partner Network (MPN) e Sviluppo/test con pagamento in base al consumo</span><span class="sxs-lookup"><span data-stu-id="38cf1-118">Transferring Visual Studio, Microsoft Partner Network (MPN) and Pay as you go Dev/Test subscriptions</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [<span data-ttu-id="38cf1-119">Domande frequenti sul trasferimento della proprietà</span><span class="sxs-lookup"><span data-stu-id="38cf1-119">Transfer Ownership FAQ</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [<span data-ttu-id="38cf1-120">Risoluzione dei problemi relativi al trasferimento della proprietà</span><span class="sxs-lookup"><span data-stu-id="38cf1-120">Troubleshoot Transfer ownership issues</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
