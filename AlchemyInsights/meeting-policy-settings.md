---
title: Impostazioni di criteri per le riunioni
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 683ca12c8f6e2511311c10ab5c4599ee66c08eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794338"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="843ec-102">Gestire i criteri di riunione in Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="843ec-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="843ec-103">**Nota: per rendere effettive le modifiche ai criteri per gli utenti, è possibile richiedere fino a 24 ore.**</span><span class="sxs-lookup"><span data-stu-id="843ec-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="843ec-104">Potrebbe non essere possibile apportare modifiche ai criteri appena creati immediatamente. attendere 4 ore e tentare di modificare nuovamente un criterio appena creato.</span><span class="sxs-lookup"><span data-stu-id="843ec-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="843ec-105">I criteri di riunione vengono utilizzati per controllare le funzionalità disponibili per i partecipanti alla riunione per le riunioni pianificate dagli utenti dell'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="843ec-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="843ec-106">Alcune funzionalità dei criteri di riunione potrebbero non essere implementate nell'interfaccia di amministrazione di Teams (queste sono etichettate come "prossimamente" nella documentazione).</span><span class="sxs-lookup"><span data-stu-id="843ec-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="843ec-107">In questo caso, o se si riceve un errore come "non è possibile aggiornare il criterio in questo momento, ma riprovare più tardi" nell'interfaccia di amministrazione di Microsoft teams, si consiglia di utilizzare PowerShell per creare o modificare i criteri di riunione dei team.</span><span class="sxs-lookup"><span data-stu-id="843ec-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="843ec-108">Per ulteriori informazioni sui criteri di riunione, vedere le risorse seguenti:</span><span class="sxs-lookup"><span data-stu-id="843ec-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="843ec-109">Per ulteriori informazioni sulla creazione di criteri, la modifica e l'assegnazione degli utenti ai criteri, vedere [Manage meeting Policies in teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="843ec-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="843ec-110">Per apportare modifiche ai criteri utilizzando i cmdlet di PowerShell, vedere [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="843ec-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="843ec-111">È necessario utilizzare il [modulo di PowerShell di Skype for business](https://www.microsoft.com/download/details.aspx?id=39366) per i criteri di riunione dei team.</span><span class="sxs-lookup"><span data-stu-id="843ec-111">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="843ec-112">Per ulteriori informazioni, vedere la [documentazione relativa ai cmdlet \*-CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) .</span><span class="sxs-lookup"><span data-stu-id="843ec-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

