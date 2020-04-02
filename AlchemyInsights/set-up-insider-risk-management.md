---
title: Configurare la gestione dei rischi Insider
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002284"
- "4405"
ms.openlocfilehash: 556150c41ccf363e6025ba6fac0660d1fb74f9b8
ms.sourcegitcommit: 92e9a649532f5231ceedcafc4d14b8ad18d517c2
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 03/31/2020
ms.locfileid: "43060002"
---
# <a name="set-up-insider-risk-management"></a><span data-ttu-id="26e74-102">Configurare la gestione dei rischi Insider</span><span class="sxs-lookup"><span data-stu-id="26e74-102">Set up insider risk management</span></span>

<span data-ttu-id="26e74-103">Usare i criteri di gestione dei rischi Insider per identificare attività rischiose e strumenti di gestione per intervenire sugli avvisi di rischio nell'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="26e74-103">Use insider risk management policies to identify risky activities and management tools to take action on risk alerts in your organization.</span></span> <span data-ttu-id="26e74-104">Prima di iniziare a usare la gestione dei rischi Insider, è necessario confermare l'**abbonamento a Microsoft 365**.</span><span class="sxs-lookup"><span data-stu-id="26e74-104">Before you get started with insider risk management, you should confirm your **Microsoft 365 subscription**.</span></span> <span data-ttu-id="26e74-105">Per accedere a e usare la gestione dei rischi Insider, **è necessario** che l'organizzazione abbia uno degli abbonamenti seguenti:</span><span class="sxs-lookup"><span data-stu-id="26e74-105">To access and use insider risk management, your organization **must** have one of the following subscriptions:</span></span>

- <span data-ttu-id="26e74-106">Abbonamento a **Microsoft 365 E5**.</span><span class="sxs-lookup"><span data-stu-id="26e74-106">**Microsoft 365 E5** subscription.</span></span>

- <span data-ttu-id="26e74-107">Abbonamento a **Microsoft 365 E3** con il componente aggiuntivo Microsoft E5 Compliance.</span><span class="sxs-lookup"><span data-stu-id="26e74-107">**Microsoft 365 E3** subscription with the Microsoft E5 compliance add-on.</span></span>

<span data-ttu-id="26e74-108">Se non si ha un piano **Microsoft 365 E5** esistente e si vuole provare la gestione dei rischi Insider, è possibile aggiungere Microsoft 365 all'abbonamento a Office 365 esistente o iscriversi a una versione di valutazione di Microsoft 365 Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="26e74-108">If you don't have an existing **Microsoft 365 E5** plan and want to try insider risk management, you can add Microsoft 365 to your existing Office 365 subscription or Sign up for a trial of Microsoft 365 Enterprise E5.</span></span>

<span data-ttu-id="26e74-109">I passaggi di base per l'uso della gestione dei rischi Insider sono:</span><span class="sxs-lookup"><span data-stu-id="26e74-109">The basic steps for using Insider Risk Management include:</span></span>

1. <span data-ttu-id="26e74-110">Abilitare le autorizzazioni per la gestione dei rischi Insider.</span><span class="sxs-lookup"><span data-stu-id="26e74-110">Enable permissions for insider risk management.</span></span>

2. <span data-ttu-id="26e74-111">Abilitare il log di controllo di Office 365.</span><span class="sxs-lookup"><span data-stu-id="26e74-111">Enable the Office 365 audit log.</span></span>

3. <span data-ttu-id="26e74-112">Configurare i prerequisiti per il modello (facoltativo).</span><span class="sxs-lookup"><span data-stu-id="26e74-112">Configure prerequisites for template (optional).</span></span>

4. <span data-ttu-id="26e74-113">Configurare le impostazioni dei rischi Insider.</span><span class="sxs-lookup"><span data-stu-id="26e74-113">Configure insider risk settings.</span></span>

5. <span data-ttu-id="26e74-114">Creare un criterio di gestione dei rischi Insider.</span><span class="sxs-lookup"><span data-stu-id="26e74-114">Create an insider risk management policy.</span></span>

<span data-ttu-id="26e74-115">Per altre informazioni sul modo in cui i criteri dei rischi Insider possono aiutare a gestire i rischi nell'organizzazione, vedere [Gestione dei rischi Insider in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2123907).</span><span class="sxs-lookup"><span data-stu-id="26e74-115">For more information about how insider risk polices can help you manage risk in your Organization, see [Insider risk management in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2123907).</span></span>
