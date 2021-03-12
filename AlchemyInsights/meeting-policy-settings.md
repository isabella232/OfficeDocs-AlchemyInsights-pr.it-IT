---
title: Impostazioni dei criteri riunione
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
ms.openlocfilehash: 24a55417df0f89063fbdd9ade6d104be4f8ab49c
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704610"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="8dd33-102">Gestire i criteri di riunione in Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="8dd33-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="8dd33-103">**Nota: l'applicazione delle modifiche ai criteri per gli utenti può richiedere fino a 24 ore.**</span><span class="sxs-lookup"><span data-stu-id="8dd33-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="8dd33-104">Potrebbe non essere possibile apportare immediatamente modifiche ai criteri appena creati. Attendere 4 ore e tentare di modificare di nuovo un criterio appena creato.</span><span class="sxs-lookup"><span data-stu-id="8dd33-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="8dd33-105">I criteri riunione vengono utilizzati per controllare le funzionalità disponibili per i partecipanti alle riunioni pianificate dagli utenti dell'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="8dd33-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="8dd33-106">Alcune funzionalità dei criteri riunione potrebbero non essere ancora implementate nell'interfaccia di amministrazione di Teams (queste sono etichettate "presto" nella documentazione).</span><span class="sxs-lookup"><span data-stu-id="8dd33-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="8dd33-107">In questo caso, o se viene visualizzato un errore come "Non è possibile aggiornare il criterio in questo momento ma riprovare in un secondo momento" nell'interfaccia di amministrazione di Microsoft Teams, è consigliabile usare PowerShell per creare o modificare i criteri di riunione di Teams.</span><span class="sxs-lookup"><span data-stu-id="8dd33-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="8dd33-108">Per ulteriori informazioni sui criteri riunione, vedere le risorse seguenti:</span><span class="sxs-lookup"><span data-stu-id="8dd33-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="8dd33-109">Per informazioni su come creare criteri, apportare modifiche e assegnare utenti ai criteri, vedere [Gestire i criteri riunione in Teams.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)</span><span class="sxs-lookup"><span data-stu-id="8dd33-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="8dd33-110">Per apportare modifiche ai criteri tramite i cmdlet di PowerShell, vedere [Panoramica di PowerShell di Teams.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)</span><span class="sxs-lookup"><span data-stu-id="8dd33-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="8dd33-111">È necessario usare il modulo [PowerShell di Skype for Business per](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) i criteri di riunione di Teams.</span><span class="sxs-lookup"><span data-stu-id="8dd33-111">You need to use the [Skype for Business PowerShell module](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="8dd33-112">Per ulteriori informazioni, vedere la documentazione relativa ai [cmdlet \*-CsTeamsMeetingPolicy.](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps)</span><span class="sxs-lookup"><span data-stu-id="8dd33-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

