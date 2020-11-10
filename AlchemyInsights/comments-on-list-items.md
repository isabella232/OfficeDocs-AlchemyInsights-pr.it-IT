---
title: Commenti sugli elementi di elenco
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003821"
- "6841"
ms.openlocfilehash: 5940d1a96324c5ca77331485a115689abe547ef7
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/09/2020
ms.locfileid: "48947507"
---
# <a name="comments-on-list-items"></a><span data-ttu-id="0d70a-102">Commenti sugli elementi di elenco</span><span class="sxs-lookup"><span data-stu-id="0d70a-102">Comments on List items</span></span>

<span data-ttu-id="0d70a-103">Gli utenti saranno presto in grado di aggiungere ed eliminare commenti sugli elementi dell'elenco.</span><span class="sxs-lookup"><span data-stu-id="0d70a-103">Users will soon be able to add and delete comments on list items.</span></span> <span data-ttu-id="0d70a-104">Gli utenti possono visualizzare tutti i commenti su un elemento di elenco e filtrare tra le visualizzazioni che mostrano commenti o attività correlate a un elemento.</span><span class="sxs-lookup"><span data-stu-id="0d70a-104">Users can view all comments on a list item and filter between views that show comments or activity related to an item.</span></span>

<span data-ttu-id="0d70a-105">**Tempistica** :</span><span class="sxs-lookup"><span data-stu-id="0d70a-105">**Timing** :</span></span>

<span data-ttu-id="0d70a-106">**Rilascio mirato** : distribuzione graduale a metà ottobre e prevista per il completamento entro la metà di novembre</span><span class="sxs-lookup"><span data-stu-id="0d70a-106">**Targeted release** : Gradual roll out in mid-October and expected to complete by mid-November</span></span>

<span data-ttu-id="0d70a-107">**Standard Release** : graduale roll out a metà novembre e previsto per il completamento entro l'inizio di dicembre</span><span class="sxs-lookup"><span data-stu-id="0d70a-107">**Standard release** : Gradual roll out in mid-November and expected to complete by early December</span></span>

<span data-ttu-id="0d70a-108">**Implementazione** : rilascio mirato per l'intera organizzazione</span><span class="sxs-lookup"><span data-stu-id="0d70a-108">**Rollout** : Targeted release for the entire organization</span></span>

<span data-ttu-id="0d70a-109">Gli utenti devono tenere presente quanto segue prima di poter aggiungere ed eliminare commenti:</span><span class="sxs-lookup"><span data-stu-id="0d70a-109">Users need to note the following before they can add and delete comments:</span></span>

- <span data-ttu-id="0d70a-110">I commenti seguono le impostazioni di autorizzazione inerenti a SharePoint.</span><span class="sxs-lookup"><span data-stu-id="0d70a-110">Comments follow the permission settings inherent in SharePoint.</span></span>
- <span data-ttu-id="0d70a-111">Gli elenchi classici che non sono ancora stati creati per essere visualizzati nelle interfacce utente moderne, come gli elenchi di attività, non avranno questa funzionalità di commento.</span><span class="sxs-lookup"><span data-stu-id="0d70a-111">Classic lists that are not yet built to show up in modern user interfaces, like task lists, will not have this commenting feature.</span></span>
- <span data-ttu-id="0d70a-112">La creazione di commenti negli elenchi dei team non è disponibile con questa versione.</span><span class="sxs-lookup"><span data-stu-id="0d70a-112">Commenting on lists in Teams is not available with this release.</span></span>
- <span data-ttu-id="0d70a-113">I commenti non vengono indicizzati dalla ricerca.</span><span class="sxs-lookup"><span data-stu-id="0d70a-113">Comments are not indexed by Search.</span></span>

<span data-ttu-id="0d70a-114">Gli amministratori possono disabilitare questa funzionalità a livello di organizzazione modificando il parametro **CommentsOnListItemsDisabled** nel cmdlet **set-SPOTenant** di PowerShell.</span><span class="sxs-lookup"><span data-stu-id="0d70a-114">Admins can disable this feature at the organization level by changing the **CommentsOnListItemsDisabled** parameter in the **Set-SPOTenant** PowerShell cmdlet.</span></span>

<span data-ttu-id="0d70a-115">Al momento non è possibile disabilitare il commento a livello di sito o di elenco.</span><span class="sxs-lookup"><span data-stu-id="0d70a-115">It is not currently possible to disable commenting at the site or list level.</span></span> <span data-ttu-id="0d70a-116">Si spera di disporre di tali controlli in un aggiornamento successivo, probabilmente nel primo trimestre 2021.</span><span class="sxs-lookup"><span data-stu-id="0d70a-116">We hope to have those controls in a later update, likely in the first quarter 2021.</span></span>
