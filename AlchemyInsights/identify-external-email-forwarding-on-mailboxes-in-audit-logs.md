---
title: Identificare l'inoltro di posta elettronica esterno nelle cassette postali nei registri di controllo
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 592eb92e4b0fe0f9da2fa20bb93ffa4fbbb76662
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508956"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="e2676-102">Identificare quando l'inoltro di posta elettronica esterno è configurato per le cassette postali</span><span class="sxs-lookup"><span data-stu-id="e2676-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="e2676-103">Quando un utente di Microsoft 365 configura l'inoltro di posta elettronica esterno su una cassetta postale, l'attività viene controllata come parte del cmdlet **Set-Mailbox** .</span><span class="sxs-lookup"><span data-stu-id="e2676-103">When a Microsoft 365 user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="e2676-104">È possibile visualizzare l'attività utilizzando la ricerca del registro di controllo nel centro sicurezza & conformità.</span><span class="sxs-lookup"><span data-stu-id="e2676-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="e2676-105">Accedere al [Centro sicurezza & conformità di Microsoft 365](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="e2676-105">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="e2676-106">Passare alla pagina di ricerca del registro di controllo della **ricerca**  >  **Audit log search** .</span><span class="sxs-lookup"><span data-stu-id="e2676-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="e2676-107">Selezionare l'intervallo di date nei campi data di **inizio** e **Data di fine** .</span><span class="sxs-lookup"><span data-stu-id="e2676-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="e2676-108">Non è necessario specificare un nome utente.</span><span class="sxs-lookup"><span data-stu-id="e2676-108">You don't need to specify a username.</span></span> <span data-ttu-id="e2676-109">Verificare che il campo **attività** sia impostato per **visualizzare i risultati di tutte le attività**.</span><span class="sxs-lookup"><span data-stu-id="e2676-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="e2676-110">Fare clic su **Cerca**.</span><span class="sxs-lookup"><span data-stu-id="e2676-110">Click **Search**.</span></span>

<span data-ttu-id="e2676-111">Nei risultati, fare clic su **Filtra risultati** e digitare **Set-Mailbox** nella casella filtro attività.</span><span class="sxs-lookup"><span data-stu-id="e2676-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="e2676-112">Selezionare un record di controllo nei risultati.</span><span class="sxs-lookup"><span data-stu-id="e2676-112">Select an audit record in the results.</span></span> <span data-ttu-id="e2676-113">Nel riquadro a comparsa **Dettagli** , fare clic su **altre informazioni**.</span><span class="sxs-lookup"><span data-stu-id="e2676-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="e2676-114">Per determinare se l'attività è correlata all'inoltro della posta elettronica, è necessario esaminare i dettagli di ogni record di controllo.</span><span class="sxs-lookup"><span data-stu-id="e2676-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="e2676-115">**ObjectID**: il valore alias della cassetta postale che è stata modificata.</span><span class="sxs-lookup"><span data-stu-id="e2676-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="e2676-116">**Parametri**: _ForwardingSmtpAddress_ indica l'indirizzo di posta elettronica di destinazione.</span><span class="sxs-lookup"><span data-stu-id="e2676-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="e2676-117">**Userid**: l'utente che ha configurato l'inoltro della posta elettronica sulla cassetta postale nel campo **ObjectID** .</span><span class="sxs-lookup"><span data-stu-id="e2676-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="e2676-118">Per ulteriori informazioni, vedere [determinare chi ha configurato l'inoltro della posta elettronica per una cassetta postale](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="e2676-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span></span>
