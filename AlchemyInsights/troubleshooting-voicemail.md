---
title: 'Risoluzione dei problemi relativi alla segreteria telefonica '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7564"
ms.openlocfilehash: a2d26da512838ae112c352fe21366074b69fa224
ms.sourcegitcommit: 3802f2f4db4f53a408a360187db67f2296448c21
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/09/2020
ms.locfileid: "49608006"
---
# <a name="troubleshooting-voicemail"></a><span data-ttu-id="4e231-102">Risoluzione dei problemi relativi alla segreteria telefonica</span><span class="sxs-lookup"><span data-stu-id="4e231-102">Troubleshooting Voicemail</span></span>

<span data-ttu-id="4e231-103">Verificare che la funzionalità occupato su occupato sia intenzionale.</span><span class="sxs-lookup"><span data-stu-id="4e231-103">Ensure that the Busy on Busy feature is intentional.</span></span>

<span data-ttu-id="4e231-104">Se questa funzionalità non è necessaria per l'utente:</span><span class="sxs-lookup"><span data-stu-id="4e231-104">If this feature is not needed on this user:</span></span>

1. <span data-ttu-id="4e231-105">Accedere a [Teams Admin Center](https://admin.teams.microsoft.com/policies/calling).</span><span class="sxs-lookup"><span data-stu-id="4e231-105">Go to [Teams Admin center](https://admin.teams.microsoft.com/policies/calling).</span></span>
1. <span data-ttu-id="4e231-106">Sul binario sinistro, i **Voice** criteri  >  di **chiamata** vocale  >  **gestiscono** i criteri nel criterio di **chiamata**.</span><span class="sxs-lookup"><span data-stu-id="4e231-106">On the left rail navigate **Voice** > **Calling policies** > **Manage Policies** on the **Calling Policy**.</span></span>
1. <span data-ttu-id="4e231-107">Selezionare **Gestisci utenti**.</span><span class="sxs-lookup"><span data-stu-id="4e231-107">Select **Manage Users**.</span></span>
1. <span data-ttu-id="4e231-108">La ricerca di un utente e la modifica del criterio di chiamata su uno che è **occupato su occupato sono disponibili quando si effettua una chiamata** a **disattivata**.</span><span class="sxs-lookup"><span data-stu-id="4e231-108">Search for user and change the Calling Policy to one that has **Busy on Busy is available when in a call** to **Off**.</span></span>
1. <span data-ttu-id="4e231-109">Fare clic su **Applica**.</span><span class="sxs-lookup"><span data-stu-id="4e231-109">Click **Apply**.</span></span>
> [!NOTE]
> <span data-ttu-id="4e231-110">Le modifiche apportate ai criteri possono richiedere fino a 24 ore per la replica.</span><span class="sxs-lookup"><span data-stu-id="4e231-110">Changes to policies can take up to 24 hours to replicate.</span></span>

<span data-ttu-id="4e231-111">Per ulteriori informazioni su questa funzionalità, vedere: [busy on busy è disponibile mentre è in una chiamata](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call).</span><span class="sxs-lookup"><span data-stu-id="4e231-111">For more information on this feature refer to: [Busy on Busy is available while in a call](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call).</span></span>
