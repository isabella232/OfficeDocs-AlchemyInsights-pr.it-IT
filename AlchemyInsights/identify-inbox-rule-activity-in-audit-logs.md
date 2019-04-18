---
title: Identificare la regola di posta in arrivo nei registri di controllo
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1368
ms.assetid: ''
ms.openlocfilehash: 9339d9c58056f568dc994b75bffe39f2c8bbdd34
ms.sourcegitcommit: ffe2f489b1ac3aae62aa784c959da6a41c3261eb
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/17/2019
ms.locfileid: "31909342"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="ebcd7-102">Identificare la regola di posta in arrivo nei registri di controllo</span><span class="sxs-lookup"><span data-stu-id="ebcd7-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="ebcd7-103">È possibile utilizzare la ricerca del registro di controllo nel centro sicurezza & Compliance per visualizzare gli eventi delle regole di posta in arrivo (creazione, modifica ed eliminazione delle regole di posta in arrivo).</span><span class="sxs-lookup"><span data-stu-id="ebcd7-103">You can use audit log search in the Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="ebcd7-104">Accedere al [centro conformità _AMP_ sicurezza di Office 365](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="ebcd7-104">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="ebcd7-105">Fare clic su **ricerca e analisi** e selezionare **Ricerca log di controllo**.</span><span class="sxs-lookup"><span data-stu-id="ebcd7-105">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="ebcd7-106">Selezionare l'intervallo di date nei campi data di **inizio** e **Data di fine** .</span><span class="sxs-lookup"><span data-stu-id="ebcd7-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="ebcd7-107">In **attività Cassetta postale di Exchange**, verificare che il campo **attività** sia impostato su **nuovo-InboxRule creare/modificare/abilitare/disabilitare la regola di posta in arrivo**.</span><span class="sxs-lookup"><span data-stu-id="ebcd7-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="ebcd7-108">Fare clic su **Cerca**.</span><span class="sxs-lookup"><span data-stu-id="ebcd7-108">Click **Search**.</span></span>

<span data-ttu-id="ebcd7-109">Nei risultati, selezionare un record di controllo.</span><span class="sxs-lookup"><span data-stu-id="ebcd7-109">In the results, select an audit record.</span></span> <span data-ttu-id="ebcd7-110">Nel riquadro a comparsa dettagli, fare clic su **altre informazioni**.</span><span class="sxs-lookup"><span data-stu-id="ebcd7-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="ebcd7-111">Le informazioni sulle impostazioni delle regole di posta in arrivo vengono visualizzate nel campo **parametri** .</span><span class="sxs-lookup"><span data-stu-id="ebcd7-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="ebcd7-112">Per ulteriori informazioni, vedere [determinare se un utente ha creato una regola di posta in arrivo](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="ebcd7-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
