---
title: Eliminare un canale privato di Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 2ee998f0c70973645c273a2a6609af2420a4f74b
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 07/28/2020
ms.locfileid: "45431617"
---
# <a name="delete-a-teams-private-channel"></a><span data-ttu-id="076ff-102">Eliminare un canale privato di Teams</span><span class="sxs-lookup"><span data-stu-id="076ff-102">Delete a Teams private channel</span></span>

<span data-ttu-id="076ff-103">Microsoft è consapevole di un problema che si verifica durante l'eliminazione di un canale privato di Teams se per il sito di SharePoint sottostante sono abilitati i criteri di conservazione di SharePoint.</span><span class="sxs-lookup"><span data-stu-id="076ff-103">Microsoft is aware of an issue deleting a Teams private channel if you have SharePoint Retention Policies enabled for the underlying SharePoint site.</span></span> <span data-ttu-id="076ff-104">Microsoft sta lavorando alla risoluzione del problema.</span><span class="sxs-lookup"><span data-stu-id="076ff-104">Microsoft is working on a fix.</span></span> <span data-ttu-id="076ff-105">Nel frattempo, è possibile provare le soluzioni alternative seguenti per eliminare il canale privato.</span><span class="sxs-lookup"><span data-stu-id="076ff-105">In the meantime, you can use the following workarounds to delete the private channel.</span></span>

<span data-ttu-id="076ff-106">**Escludere il Team o la raccolta siti dai criteri di conservazione di SharePoint.**</span><span class="sxs-lookup"><span data-stu-id="076ff-106">**Exclude the Team/site collection from the Sharepoint retention policy.**</span></span>

1. <span data-ttu-id="076ff-107">Passare al portale di amministrazione di Office 365 e selezionare **Mostra tutto** nel riquadro di spostamento sinistro.</span><span class="sxs-lookup"><span data-stu-id="076ff-107">Go to the Office 365 admin portal, and select **Show all** in the left navigation pane.</span></span>
2. <span data-ttu-id="076ff-108">In **Interfacce di amministrazione**, selezionare **Sicurezza e conformità** > **Prevenzione della perdita dei dati** > **Criteri**.</span><span class="sxs-lookup"><span data-stu-id="076ff-108">Under **Admin centers**, go to **Security & Compliance** > **Data Loss Prevention** > **Policy**.</span></span>
3. <span data-ttu-id="076ff-109">Identificare i criteri applicabili ai siti di SharePoint e modificarli in modo che il sito di SharePoint per il Team contenente il canale privato NON sia incluso nei criteri di conservazione.</span><span class="sxs-lookup"><span data-stu-id="076ff-109">Identify any policy that applies to Sharepoint sites, and modify the policy so the Sharepoint site for the Team containing the private channel is NOT included under the retention policy.</span></span>
4. <span data-ttu-id="076ff-110">Salvare il criterio.</span><span class="sxs-lookup"><span data-stu-id="076ff-110">Save the policy.</span></span>
    <span data-ttu-id="076ff-111">Possono essere necessarie fino a 24 ore prima che le impostazioni dei criteri diventino effettive.</span><span class="sxs-lookup"><span data-stu-id="076ff-111">It can take up to 24 hours for policy settings to take effect.</span></span>
    <span data-ttu-id="076ff-112">Una volta escluso il sito, è possibile eliminare il canale privato.</span><span class="sxs-lookup"><span data-stu-id="076ff-112">After the site has been excluded, you can delete the private channel.</span></span>  
    
<span data-ttu-id="076ff-113">È ***possibile*** eliminare il canale privato usando Microsoft Teams sul dispositivo Android.</span><span class="sxs-lookup"><span data-stu-id="076ff-113">You  ***might*** be able to delete the private channel by using Microsoft Teams on your Android device.</span></span> 

<span data-ttu-id="076ff-114">Per informazioni collegate a SharePoint, si veda [Non è possibile eliminare elementi in SharePoint Online o OneDrive for Business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span><span class="sxs-lookup"><span data-stu-id="076ff-114">For related SharePoint information, see [Unable to delete items in SharePoint Online or OneDrive for Business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span></span>