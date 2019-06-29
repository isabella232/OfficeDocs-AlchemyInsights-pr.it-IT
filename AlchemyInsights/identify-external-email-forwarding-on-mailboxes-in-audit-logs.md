---
title: Identificare l'inoltro di posta elettronica esterno nelle cassette postali nei registri di controllo
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 43b6a26bc05892e71d41c4b47522785245cb4851
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/28/2019
ms.locfileid: "35383101"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="79659-102">Identificare quando l'inoltro di posta elettronica esterno è configurato per le cassette postali</span><span class="sxs-lookup"><span data-stu-id="79659-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="79659-103">Quando un utente configura l'inoltro di posta elettronica esterno su una cassetta postale, l'attività viene controllata come parte del cmdlet **Set-Mailbox** .</span><span class="sxs-lookup"><span data-stu-id="79659-103">When a user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="79659-104">È possibile visualizzare l'attività utilizzando la ricerca del registro di controllo nel centro sicurezza & conformità.</span><span class="sxs-lookup"><span data-stu-id="79659-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="79659-105">Accedere al [Centro sicurezza & conformità di Office 365](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="79659-105">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="79659-106">Fare clic su **ricerca e analisi** e selezionare **Ricerca log di controllo**.</span><span class="sxs-lookup"><span data-stu-id="79659-106">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="79659-107">Selezionare l'intervallo di date nei campi data di **inizio** e **Data di fine** .</span><span class="sxs-lookup"><span data-stu-id="79659-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="79659-108">Non è necessario specificare un nome utente.</span><span class="sxs-lookup"><span data-stu-id="79659-108">You don't need to specify a username.</span></span> <span data-ttu-id="79659-109">Verificare che il campo **attività** sia impostato per **visualizzare i risultati di tutte le attività**.</span><span class="sxs-lookup"><span data-stu-id="79659-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="79659-110">Fare clic su **Cerca**.</span><span class="sxs-lookup"><span data-stu-id="79659-110">Click **Search**.</span></span>

<span data-ttu-id="79659-111">Nei risultati, fare clic su **Filtra risultati** e digitare **Set-Mailbox** nella casella filtro attività.</span><span class="sxs-lookup"><span data-stu-id="79659-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="79659-112">Selezionare un record di controllo nei risultati.</span><span class="sxs-lookup"><span data-stu-id="79659-112">Select an audit record in the results.</span></span> <span data-ttu-id="79659-113">Nel riquadro a comparsa **Dettagli** , fare clic su **altre informazioni**.</span><span class="sxs-lookup"><span data-stu-id="79659-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="79659-114">Per determinare se l'attività è correlata all'inoltro della posta elettronica, è necessario esaminare i dettagli di ogni record di controllo.</span><span class="sxs-lookup"><span data-stu-id="79659-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="79659-115">**ObjectID**: il valore alias della cassetta postale che è stata modificata.</span><span class="sxs-lookup"><span data-stu-id="79659-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="79659-116">**Parametri**: _ForwardingSmtpAddress_ indica l'indirizzo di posta elettronica di destinazione.</span><span class="sxs-lookup"><span data-stu-id="79659-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="79659-117">**Userid**: l'utente che ha configurato l'inoltro della posta elettronica sulla cassetta postale nel campo **ObjectID** .</span><span class="sxs-lookup"><span data-stu-id="79659-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="79659-118">Per ulteriori informazioni, vedere [determinare chi ha configurato l'inoltro della posta elettronica per una cassetta postale](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="79659-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span></span>
