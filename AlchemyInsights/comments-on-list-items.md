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
ms.openlocfilehash: 2ee95e98aae3d9ec9a933f9cae234111d4285edd
ms.sourcegitcommit: 2eb1dd0856509b9907ccba9a5cb99d09b4f6eb4b
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/21/2020
ms.locfileid: "49724158"
---
# <a name="comments-on-list-items"></a><span data-ttu-id="038b4-102">Commenti sugli elementi di elenco</span><span class="sxs-lookup"><span data-stu-id="038b4-102">Comments on List items</span></span>

<span data-ttu-id="038b4-103">Gli utenti possono visualizzare tutti i commenti su un elemento di elenco e filtrare tra le visualizzazioni che mostrano commenti o attività correlate a un elemento.</span><span class="sxs-lookup"><span data-stu-id="038b4-103">Users can view all comments on a list item and filter between views that show comments or activity related to an item.</span></span>

<span data-ttu-id="038b4-104">Gli utenti devono tenere presente quanto segue prima di poter aggiungere ed eliminare commenti:</span><span class="sxs-lookup"><span data-stu-id="038b4-104">Users need to note the following before they can add and delete comments:</span></span>

- <span data-ttu-id="038b4-105">I commenti seguono le impostazioni di autorizzazione inerenti a SharePoint.</span><span class="sxs-lookup"><span data-stu-id="038b4-105">Comments follow the permission settings inherent in SharePoint.</span></span>
- <span data-ttu-id="038b4-106">Gli elenchi classici che non sono ancora stati creati per essere visualizzati nelle interfacce utente moderne, come gli elenchi di attività, non avranno questa funzionalità di commento.</span><span class="sxs-lookup"><span data-stu-id="038b4-106">Classic lists that are not yet built to show up in modern user interfaces, like task lists, will not have this commenting feature.</span></span>
- <span data-ttu-id="038b4-107">La creazione di commenti negli elenchi dei team non è disponibile con questa versione.</span><span class="sxs-lookup"><span data-stu-id="038b4-107">Commenting on lists in Teams is not available with this release.</span></span>
- <span data-ttu-id="038b4-108">I commenti non vengono indicizzati dalla ricerca.</span><span class="sxs-lookup"><span data-stu-id="038b4-108">Comments are not indexed by Search.</span></span>

<span data-ttu-id="038b4-109">Gli amministratori possono disabilitare questa funzionalità a livello di organizzazione modificando il parametro **CommentsOnListItemsDisabled** nel cmdlet **set-SPOTenant** di PowerShell.</span><span class="sxs-lookup"><span data-stu-id="038b4-109">Admins can disable this feature at the organization level by changing the **CommentsOnListItemsDisabled** parameter in the **Set-SPOTenant** PowerShell cmdlet.</span></span>

<span data-ttu-id="038b4-110">Al momento non è possibile disabilitare il commento a livello di sito o di elenco.</span><span class="sxs-lookup"><span data-stu-id="038b4-110">It is not currently possible to disable commenting at the site or list level.</span></span> <span data-ttu-id="038b4-111">Si spera di disporre di tali controlli in un aggiornamento successivo, probabilmente nel primo trimestre 2021.</span><span class="sxs-lookup"><span data-stu-id="038b4-111">We hope to have those controls in a later update, likely in the first quarter 2021.</span></span>
