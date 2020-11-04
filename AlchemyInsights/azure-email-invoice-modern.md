---
title: Fatturazione moderna di Azure tramite posta elettronica
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
- "9003801"
- "6866"
ms.openlocfilehash: 65df6091a97d4937379ded384a78b5d07aa76e42
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 11/03/2020
ms.locfileid: "48840602"
---
# <a name="email-invoicing-in-azure"></a><span data-ttu-id="9a47d-102">Fatturazione di Azure tramite posta elettronica</span><span class="sxs-lookup"><span data-stu-id="9a47d-102">Email invoicing in Azure</span></span>

<span data-ttu-id="9a47d-103">Per aggiornare le preferenze per la fatturazione tramite posta elettronica, è necessario disporre del ruolo di proprietario o collaboratore nel profilo o nell'account di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="9a47d-103">You must have an owner or a contributor role on the billing profile or its billing account to update its email invoice preference.</span></span> <span data-ttu-id="9a47d-104">Dopo aver accettato esplicitamente, tutti gli utenti con il ruolo di proprietario, collaboratore, lettore e responsabile della fatturazione nel profilo di fatturazione riceveranno la fattura tramite posta elettronica.</span><span class="sxs-lookup"><span data-stu-id="9a47d-104">Once you have opted-in, all users with an owner, contributor, readers, and invoice manager roles on a billing profile will get its invoice in email.</span></span>

1. <span data-ttu-id="9a47d-105">Accedere al [portale di Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="9a47d-105">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="9a47d-106">Cercare **Gestione costi e fatturazione**.</span><span class="sxs-lookup"><span data-stu-id="9a47d-106">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="9a47d-107">Selezionare **Fatture** nel lato sinistro e quindi selezionare **Fattura per posta elettronica** nella parte superiore della pagina.</span><span class="sxs-lookup"><span data-stu-id="9a47d-107">Select **Invoices** from the left-hand side and then select **Email Invoice** from the top of the page.</span></span>
4. <span data-ttu-id="9a47d-108">Se si hanno più profili di fatturazione, selezionare un profilo e quindi selezionare **Acconsento esplicitamente**.</span><span class="sxs-lookup"><span data-stu-id="9a47d-108">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

5. <span data-ttu-id="9a47d-109">Selezionare **Aggiorna**.</span><span class="sxs-lookup"><span data-stu-id="9a47d-109">Select **Update**.</span></span>
6. <span data-ttu-id="9a47d-110">Se si hanno più profili di fatturazione, selezionare un profilo e quindi selezionare **Acconsento esplicitamente**.</span><span class="sxs-lookup"><span data-stu-id="9a47d-110">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

<span data-ttu-id="9a47d-111">È possibile concedere ad altri utenti l'accesso alla visualizzazione, al download e al pagamento delle fatture assegnando loro il ruolo di responsabile per un profilo di fatturazione MCA o MPA.</span><span class="sxs-lookup"><span data-stu-id="9a47d-111">You give others access to view, download, and pay invoices by assigning them the invoice manager role for an MCA or MPA billing profile.</span></span> <span data-ttu-id="9a47d-112">Se si è scelto di ricevere le fatture tramite posta elettronica, anche gli utenti riceveranno le fatture tramite posta elettronica.</span><span class="sxs-lookup"><span data-stu-id="9a47d-112">If you've opted in to get your invoice in email, users also get the invoices in email.</span></span>

1. <span data-ttu-id="9a47d-113">Accedere al [portale di Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="9a47d-113">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="9a47d-114">Cercare **Gestione costi e fatturazione**.</span><span class="sxs-lookup"><span data-stu-id="9a47d-114">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="9a47d-115">Selezionare **Profili di fatturazione** nel lato sinistro.</span><span class="sxs-lookup"><span data-stu-id="9a47d-115">Select **Billing profiles** from the left-hand side.</span></span> <span data-ttu-id="9a47d-116">Nell'elenco dei profili fatturazione, selezionare un profilo per il quale si vuole assegnare un ruolo di responsabile della fatturazione.</span><span class="sxs-lookup"><span data-stu-id="9a47d-116">From the billing profiles list, select a billing profile for which you want to assign an invoice manager role.</span></span>
4. <span data-ttu-id="9a47d-117">Selezionare **Controllo di accesso (IAM)** nel lato sinistro e quindi selezionare **Aggiungi** nella parte superiore della pagina.</span><span class="sxs-lookup"><span data-stu-id="9a47d-117">Select **Access Control (IAM)** from the left-hand side and then select **Add** from the top of the page.</span></span>

<span data-ttu-id="9a47d-118">Nell'elenco a discesa Ruolo, selezionare **Responsabile per la fatturazione**.</span><span class="sxs-lookup"><span data-stu-id="9a47d-118">In the Role drop-down list, select **Invoice Manager**.</span></span> <span data-ttu-id="9a47d-119">Immettere l'indirizzo di posta elettronica dell'utente a cui si vuole concedere l'accesso.</span><span class="sxs-lookup"><span data-stu-id="9a47d-119">Enter the email address of the user to give access.</span></span> <span data-ttu-id="9a47d-120">Selezionare **Salva** per assegnare il ruolo.</span><span class="sxs-lookup"><span data-stu-id="9a47d-120">Select **Save** to assign the role.</span></span>
