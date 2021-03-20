---
title: Impedire all'utente di registrare riunioni
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "9325"
ms.openlocfilehash: 3f633ee1fb3329b6fc634acabbc824af1eccfb33
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897980"
---
# <a name="block-user-from-recording-meetings"></a><span data-ttu-id="955df-102">Impedire all'utente di registrare riunioni</span><span class="sxs-lookup"><span data-stu-id="955df-102">Block User From Recording Meetings</span></span>

<span data-ttu-id="955df-103">Se è necessario impedire **o impedire** a utenti specifici di registrare riunioni di Teams, è possibile farlo tramite le impostazioni dei criteri riunione di Teams.</span><span class="sxs-lookup"><span data-stu-id="955df-103">If you need to **prevent or block** specific users from recording Teams Meetings, you can do so via Teams Meeting Policy settings.</span></span> <span data-ttu-id="955df-104">Nell'interfaccia di amministrazione di Microsoft Teams disattivare l'impostazione Consenti registrazione **cloud** nel criterio riunione assegnato a tale utente.</span><span class="sxs-lookup"><span data-stu-id="955df-104">In the Microsoft Teams admin center, turn off the **Allow cloud recording** setting in the meeting policy assigned to that user.</span></span> <span data-ttu-id="955df-105">Per ulteriori informazioni, vedere [Manage meeting policies in Teams.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-cloud-recording)</span><span class="sxs-lookup"><span data-stu-id="955df-105">To learn more, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-cloud-recording).</span></span>

<span data-ttu-id="955df-106">Per verificare se a un utente specifico è consentito o meno registrare riunioni di Teams, utilizzare la diagnostica di supporto.</span><span class="sxs-lookup"><span data-stu-id="955df-106">To validate if a specific user is allowed or not to record Teams Meetings, use the support diagnostic.</span></span> <span data-ttu-id="955df-107">Eseguire una nuova query di supporto e digitare **Diag: Registrazione** riunione: la diagnostica controlla le impostazioni dei criteri per l'utente specificato e ne determina le impostazioni.</span><span class="sxs-lookup"><span data-stu-id="955df-107">Run a new support query and type in **Diag: Meeting Recording** - the diagnostic will check policy settings for the specified user and determine their policy settings.</span></span> <span data-ttu-id="955df-108">Tenere presente che l'applicazione delle nuove impostazioni dei criteri può richiedere un paio d'ore, quindi se è stata appena apportata una modifica, attendere alcune ore prima di eseguire di nuovo la diagnostica.</span><span class="sxs-lookup"><span data-stu-id="955df-108">Remember, it can take a couple of hours for new policy settings to take effect, so if you have just made a change, wait a few hours before running the diagnostic again.</span></span>

<span data-ttu-id="955df-109">Per ulteriori informazioni, vedere [Attivare o disattivare la registrazione cloud.](https://docs.microsoft.com/microsoftteams/cloud-recording#turn-on-or-turn-off-cloud-recording)</span><span class="sxs-lookup"><span data-stu-id="955df-109">For more information, review [Turn on or turn off cloud recording](https://docs.microsoft.com/microsoftteams/cloud-recording#turn-on-or-turn-off-cloud-recording).</span></span>
