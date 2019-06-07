---
title: Identificare la regola di posta in arrivo nei registri di controllo
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1368
ms.assetid: ''
ms.openlocfilehash: f130846dd24cef81177934aa2a200c1056172d3f
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/07/2019
ms.locfileid: "34755042"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="39b02-102">Identificare la regola di posta in arrivo nei registri di controllo</span><span class="sxs-lookup"><span data-stu-id="39b02-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="39b02-103">È possibile utilizzare la ricerca del registro di controllo nel centro sicurezza & conformità per visualizzare gli eventi delle regole di posta in arrivo (creazione, modifica ed eliminazione delle regole di posta in arrivo).</span><span class="sxs-lookup"><span data-stu-id="39b02-103">You can use audit log search in the Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="39b02-104">Accedere al [Centro sicurezza & conformità di Office 365](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="39b02-104">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="39b02-105">Fare clic su **ricerca e analisi** e selezionare **Ricerca log di controllo**.</span><span class="sxs-lookup"><span data-stu-id="39b02-105">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="39b02-106">Selezionare l'intervallo di date nei campi data di **inizio** e **Data di fine** .</span><span class="sxs-lookup"><span data-stu-id="39b02-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="39b02-107">In **attività Cassetta postale di Exchange**, verificare che il campo **attività** sia impostato su **nuovo-InboxRule creare/modificare/abilitare/disabilitare la regola di posta in arrivo**.</span><span class="sxs-lookup"><span data-stu-id="39b02-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="39b02-108">Fare clic su **Cerca**.</span><span class="sxs-lookup"><span data-stu-id="39b02-108">Click **Search**.</span></span>

<span data-ttu-id="39b02-109">Nei risultati, selezionare un record di controllo.</span><span class="sxs-lookup"><span data-stu-id="39b02-109">In the results, select an audit record.</span></span> <span data-ttu-id="39b02-110">Nel riquadro a comparsa dettagli, fare clic su **altre informazioni**.</span><span class="sxs-lookup"><span data-stu-id="39b02-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="39b02-111">Le informazioni sulle impostazioni delle regole di posta in arrivo vengono visualizzate nel campo **parametri** .</span><span class="sxs-lookup"><span data-stu-id="39b02-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="39b02-112">Per ulteriori informazioni, vedere [determinare se un utente ha creato una regola di posta in arrivo](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="39b02-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
