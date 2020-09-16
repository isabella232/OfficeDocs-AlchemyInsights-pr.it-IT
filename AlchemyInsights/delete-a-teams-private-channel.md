---
title: Eliminare un canale privato di Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 56021a335c64810700913cf08519b95f24a7a17d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47730919"
---
# <a name="delete-a-teams-private-channel"></a><span data-ttu-id="86165-102">Eliminare un canale privato di Teams</span><span class="sxs-lookup"><span data-stu-id="86165-102">Delete a Teams private channel</span></span>

<span data-ttu-id="86165-103">Microsoft è consapevole di un problema che si verifica durante l'eliminazione di un canale privato di Teams se per il sito di SharePoint sottostante sono abilitati i criteri di conservazione di SharePoint.</span><span class="sxs-lookup"><span data-stu-id="86165-103">Microsoft is aware of an issue deleting a Teams private channel if you have SharePoint Retention Policies enabled for the underlying SharePoint site.</span></span> <span data-ttu-id="86165-104">Microsoft sta lavorando alla risoluzione del problema.</span><span class="sxs-lookup"><span data-stu-id="86165-104">Microsoft is working on a fix.</span></span> <span data-ttu-id="86165-105">Nel frattempo, è possibile provare le soluzioni alternative seguenti per eliminare il canale privato.</span><span class="sxs-lookup"><span data-stu-id="86165-105">In the meantime, you can use the following workarounds to delete the private channel.</span></span>

<span data-ttu-id="86165-106">**Escludere il Team o la raccolta siti dai criteri di conservazione di SharePoint.**</span><span class="sxs-lookup"><span data-stu-id="86165-106">**Exclude the Team/site collection from the Sharepoint retention policy.**</span></span>

1. <span data-ttu-id="86165-107">Passare al portale di amministrazione di Office 365 e selezionare **Mostra tutto** nel riquadro di spostamento sinistro.</span><span class="sxs-lookup"><span data-stu-id="86165-107">Go to the Office 365 admin portal, and select **Show all** in the left navigation pane.</span></span>
2. <span data-ttu-id="86165-108">In **Interfacce di amministrazione**, selezionare **Sicurezza e conformità** > **Prevenzione della perdita dei dati** > **Criteri**.</span><span class="sxs-lookup"><span data-stu-id="86165-108">Under **Admin centers**, go to **Security & Compliance** > **Data Loss Prevention** > **Policy**.</span></span>
3. <span data-ttu-id="86165-109">Identificare i criteri applicabili ai siti di SharePoint e modificarli in modo che il sito di SharePoint per il Team contenente il canale privato NON sia incluso nei criteri di conservazione.</span><span class="sxs-lookup"><span data-stu-id="86165-109">Identify any policy that applies to Sharepoint sites, and modify the policy so the Sharepoint site for the Team containing the private channel is NOT included under the retention policy.</span></span>
4. <span data-ttu-id="86165-110">Salvare il criterio.</span><span class="sxs-lookup"><span data-stu-id="86165-110">Save the policy.</span></span>
    <span data-ttu-id="86165-111">Possono essere necessarie fino a 24 ore prima che le impostazioni dei criteri diventino effettive.</span><span class="sxs-lookup"><span data-stu-id="86165-111">It can take up to 24 hours for policy settings to take effect.</span></span>
    <span data-ttu-id="86165-112">Una volta escluso il sito, è possibile eliminare il canale privato.</span><span class="sxs-lookup"><span data-stu-id="86165-112">After the site has been excluded, you can delete the private channel.</span></span>  
    
<span data-ttu-id="86165-113">È ***possibile*** eliminare il canale privato usando Microsoft Teams sul dispositivo Android.</span><span class="sxs-lookup"><span data-stu-id="86165-113">You  ***might*** be able to delete the private channel by using Microsoft Teams on your Android device.</span></span> 

<span data-ttu-id="86165-114">Per informazioni collegate a SharePoint, si veda [Non è possibile eliminare elementi in SharePoint Online o OneDrive for Business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span><span class="sxs-lookup"><span data-stu-id="86165-114">For related SharePoint information, see [Unable to delete items in SharePoint Online or OneDrive for Business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span></span>