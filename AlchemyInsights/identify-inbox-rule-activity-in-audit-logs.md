---
title: Identificare la regola di posta in arrivo nei registri di controllo
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: f946510539b3d28f2ceeec1546cbffce8bd352fd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716428"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="fb3bf-102">Identificare la regola di posta in arrivo nei registri di controllo</span><span class="sxs-lookup"><span data-stu-id="fb3bf-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="fb3bf-103">È possibile utilizzare la ricerca del registro di controllo nel centro sicurezza & conformità di Microsoft 365 per visualizzare gli eventi delle regole di posta in arrivo (creazione, modifica ed eliminazione delle regole di posta in arrivo).</span><span class="sxs-lookup"><span data-stu-id="fb3bf-103">You can use audit log search in the Microsoft 365 Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="fb3bf-104">Accedere al [Centro sicurezza & conformità di Microsoft 365](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="fb3bf-104">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="fb3bf-105">Passare alla pagina di**ricerca del registro di controllo** della **ricerca** > .</span><span class="sxs-lookup"><span data-stu-id="fb3bf-105">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="fb3bf-106">Selezionare l'intervallo di date nei campi data di **inizio** e **Data di fine** .</span><span class="sxs-lookup"><span data-stu-id="fb3bf-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="fb3bf-107">In **attività Cassetta postale di Exchange**, verificare che il campo **attività** sia impostato su **nuovo-InboxRule creare/modificare/abilitare/disabilitare la regola di posta in arrivo**.</span><span class="sxs-lookup"><span data-stu-id="fb3bf-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="fb3bf-108">Fare clic su **Cerca**.</span><span class="sxs-lookup"><span data-stu-id="fb3bf-108">Click **Search**.</span></span>

<span data-ttu-id="fb3bf-109">Nei risultati, selezionare un record di controllo.</span><span class="sxs-lookup"><span data-stu-id="fb3bf-109">In the results, select an audit record.</span></span> <span data-ttu-id="fb3bf-110">Nel riquadro a comparsa dettagli, fare clic su **altre informazioni**.</span><span class="sxs-lookup"><span data-stu-id="fb3bf-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="fb3bf-111">Le informazioni sulle impostazioni delle regole di posta in arrivo vengono visualizzate nel campo **parametri** .</span><span class="sxs-lookup"><span data-stu-id="fb3bf-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="fb3bf-112">Per ulteriori informazioni, vedere [determinare se un utente ha creato una regola di posta in arrivo](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="fb3bf-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
