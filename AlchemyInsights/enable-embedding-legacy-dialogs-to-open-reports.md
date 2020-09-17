---
title: Abilitare l'incorporamento delle finestre di dialogo legacy per aprire i report
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: 285933e607ac7e58256709f0c9cf2851250ce211
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806439"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a><span data-ttu-id="a27d6-102">Abilitare l'incorporamento delle finestre di dialogo legacy per aprire i report</span><span class="sxs-lookup"><span data-stu-id="a27d6-102">Enable embedding legacy dialogs to open reports</span></span>

<span data-ttu-id="a27d6-103">**Sintomo**</span><span class="sxs-lookup"><span data-stu-id="a27d6-103">**Symptom**</span></span>

<span data-ttu-id="a27d6-104">Gli utenti non possono aprire i report.</span><span class="sxs-lookup"><span data-stu-id="a27d6-104">Users are unable to open reports.</span></span> <span data-ttu-id="a27d6-105">“Si è verificato un errore.</span><span class="sxs-lookup"><span data-stu-id="a27d6-105">"Something has gone wrong.</span></span> <span data-ttu-id="a27d6-106">Controlla i dettagli tecnici per ulteriori informazioni.”</span><span class="sxs-lookup"><span data-stu-id="a27d6-106">Check technical details for more details."</span></span>

<span data-ttu-id="a27d6-107">**Causa**</span><span class="sxs-lookup"><span data-stu-id="a27d6-107">**Cause**</span></span>

<span data-ttu-id="a27d6-108">I report non riescono a caricarsi in UCI con l'errore "Il descrittore di modulo è nullo o non definito."</span><span class="sxs-lookup"><span data-stu-id="a27d6-108">Reports are failing to load in UCI with the error, "Form descriptor is null or not defined."</span></span> <span data-ttu-id="a27d6-109">I report in UCI richiedono ancora le finestre di dialogo legacy, pertanto il sistema del cliente deve avere *allowlegacydialogsembedding*abilitato.</span><span class="sxs-lookup"><span data-stu-id="a27d6-109">Reports in UCI still require legacy dialogs, so the customer's system needs to have *allowlegacydialogsembedding* enabled.</span></span>

<span data-ttu-id="a27d6-110">**Soluzione**</span><span class="sxs-lookup"><span data-stu-id="a27d6-110">**Solution**</span></span>

1. <span data-ttu-id="a27d6-111">Passare a **Impostazioni > Amministrazione > Impostazioni di sistema > Scheda generale**.</span><span class="sxs-lookup"><span data-stu-id="a27d6-111">Go to **Settings >Administration > System Settings > General tab**.</span></span>

2. <span data-ttu-id="a27d6-112">Impostare "Abilita incorporamento di alcune finestre di dialogo legacy nel client del browser delle interfacce unificate" su **Sì**.</span><span class="sxs-lookup"><span data-stu-id="a27d6-112">Set "Enable embedding of certain legacy dialogs in Unified Interface browser client" to **Yes**.</span></span>
