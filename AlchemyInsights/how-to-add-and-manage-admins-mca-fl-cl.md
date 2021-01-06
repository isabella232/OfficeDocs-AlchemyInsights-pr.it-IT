---
title: Come aggiungere e gestire gli amministratori
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
- "9004114"
- "7424"
ms.openlocfilehash: 25fc25392778ae71ec0553e8d8718ec487738acb
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755499"
---
# <a name="how-to-add-and-manage-admins"></a><span data-ttu-id="644cd-102">Come aggiungere e gestire gli amministratori</span><span class="sxs-lookup"><span data-stu-id="644cd-102">How to add and manage admins</span></span>

<span data-ttu-id="644cd-103">In base alla descrizione del problema, è stata trovata una soluzione per l'utente.</span><span class="sxs-lookup"><span data-stu-id="644cd-103">Based on your issue description, we’ve found a solution for you.</span></span> <span data-ttu-id="644cd-104">La maggior parte dei clienti è stata in grado di risolvere il problema da solo dopo aver seguito la nostra documentazione.</span><span class="sxs-lookup"><span data-stu-id="644cd-104">Most customers were able to resolve their issue on their own after following our documentation.</span></span>

<span data-ttu-id="644cd-105">Per gestire l'account di fatturazione per un contratto per i clienti Microsoft (MCA), è possibile utilizzare ruoli diversi con il livello di accesso desiderato.</span><span class="sxs-lookup"><span data-stu-id="644cd-105">To manage your billing account for a Microsoft Customer Agreement (MCA), you can use different roles with the desired level of access.</span></span> <span data-ttu-id="644cd-106">Questi ruoli sono oltre ai ruoli del servizio Azure incorporati che consentono di controllare le risorse.</span><span class="sxs-lookup"><span data-stu-id="644cd-106">These roles are in addition to the built-in Azure service roles which help you control your resources.</span></span>

<span data-ttu-id="644cd-107">**Per aggiungere ruoli di fatturazione nel portale di Azure:**</span><span class="sxs-lookup"><span data-stu-id="644cd-107">**To add billing roles in the Azure portal:**</span></span>

1. <span data-ttu-id="644cd-108">Accedere al [portale di Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="644cd-108">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="644cd-109">Ricerca per la *gestione dei costi + fatturazione*.</span><span class="sxs-lookup"><span data-stu-id="644cd-109">Search for *Cost Management + Billing*.</span></span>
3. <span data-ttu-id="644cd-110">Selezionare controllo di accesso (IAM) in un ambito, ad esempio account di fatturazione, profilo di fatturazione o sezione fattura in cui si desidera concedere l'accesso.</span><span class="sxs-lookup"><span data-stu-id="644cd-110">Select Access control (IAM) at a scope such as billing account, billing profile, or invoice section where you want to give access.</span></span>
4. <span data-ttu-id="644cd-111">La pagina di controllo di accesso (IAM) elenca gli utenti e i gruppi assegnati a ogni ruolo per tale ambito.</span><span class="sxs-lookup"><span data-stu-id="644cd-111">The Access control (IAM) page lists users and groups that are assigned to each role for that scope.</span></span>
5. <span data-ttu-id="644cd-112">Per concedere l'accesso a un utente, selezionare **Aggiungi** dalla parte superiore della pagina.</span><span class="sxs-lookup"><span data-stu-id="644cd-112">To give access to a user, select **Add** from the top of the page.</span></span> <span data-ttu-id="644cd-113">Nell'elenco a discesa *ruolo* selezionare un ruolo.</span><span class="sxs-lookup"><span data-stu-id="644cd-113">In the *Role* drop-down list, select a role.</span></span> <span data-ttu-id="644cd-114">Immettere l'indirizzo di posta elettronica dell'utente a cui si desidera concedere l'accesso.</span><span class="sxs-lookup"><span data-stu-id="644cd-114">Enter the email address of the user to whom you want to give access.</span></span> <span data-ttu-id="644cd-115">Selezionare **Salva** per assegnare il ruolo.</span><span class="sxs-lookup"><span data-stu-id="644cd-115">Select **Save** to assign the role.</span></span>
6. <span data-ttu-id="644cd-116">Per rimuovere l'accesso per un utente, selezionare l'utente con l'assegnazione di ruolo che si desidera rimuovere.</span><span class="sxs-lookup"><span data-stu-id="644cd-116">To remove access for a user, select the user with the role assignment you want to remove.</span></span> <span data-ttu-id="644cd-117">Selezionare **Rimuovi**.</span><span class="sxs-lookup"><span data-stu-id="644cd-117">Select **Remove**.</span></span>

<span data-ttu-id="644cd-118">**Documenti consigliati**</span><span class="sxs-lookup"><span data-stu-id="644cd-118">**Recommended Documents**</span></span>

- [<span data-ttu-id="644cd-119">Definizioni del ruolo di fatturazione</span><span class="sxs-lookup"><span data-stu-id="644cd-119">Billing role definitions</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles)
- [<span data-ttu-id="644cd-120">Ruoli e attività dell'account di fatturazione</span><span class="sxs-lookup"><span data-stu-id="644cd-120">Billing account roles and tasks</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles#billing-account-roles-and-tasks)
- [<span data-ttu-id="644cd-121">Iniziare a usare il proprio account di fatturazione MCA</span><span class="sxs-lookup"><span data-stu-id="644cd-121">Get started with your MCA billing account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/understand/mca-overview)
- [<span data-ttu-id="644cd-122">Controllare l'accesso a un contratto per i clienti Microsoft</span><span class="sxs-lookup"><span data-stu-id="644cd-122">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support%22%20%5Cl%20%22manage-credit-cards-for-a-microsoft-customer-agreement%22%20%5Ct%20%22_blank#check-the-type-of-your-account)
