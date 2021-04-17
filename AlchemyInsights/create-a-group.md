---
title: Creare un gruppo
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816360"
---
# <a name="create-a-group"></a><span data-ttu-id="b980d-102">Creare un gruppo</span><span class="sxs-lookup"><span data-stu-id="b980d-102">Create a group</span></span>

<span data-ttu-id="b980d-103">In questo argomento viene descritta la creazione di gruppi.</span><span class="sxs-lookup"><span data-stu-id="b980d-103">This topic describes group creation.</span></span>

<span data-ttu-id="b980d-104">**Autorizzazione per la creazione di un gruppo**</span><span class="sxs-lookup"><span data-stu-id="b980d-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="b980d-105">Assicurarsi di essere autorizzati a creare un nuovo gruppo.</span><span class="sxs-lookup"><span data-stu-id="b980d-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="b980d-106">Gli amministratori globali possono disabilitare la creazione di gruppi nel portale di Azure o nel riquadro di accesso.</span><span class="sxs-lookup"><span data-stu-id="b980d-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="b980d-107">Potrebbe essere necessario un amministratore per creare il nuovo gruppo o per farsi assegnare le autorizzazioni appropriate.</span><span class="sxs-lookup"><span data-stu-id="b980d-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="b980d-108">**Gestire le autorizzazioni per la creazione di gruppi**</span><span class="sxs-lookup"><span data-stu-id="b980d-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="b980d-109">Gli amministratori globali possono gestire le autorizzazioni per la creazione di gruppi (per motivi di sicurezza) o i gruppi di Office 365 creati nel portale di Azure o nel pannello di accesso, scegliendo "Gli utenti possono creare gruppi di sicurezza nei portali di Azure" o "Gli utenti possono creare gruppi di Office 365 nei portali di Azure" in **Tutti** i gruppi  >  **Generale (Impostazioni).**</span><span class="sxs-lookup"><span data-stu-id="b980d-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="b980d-110">È inoltre possibile limitare la creazione di gruppi per selezionare un gruppo di utenti se si dispone di una licenza di Azure Active Directory P1 Premium.</span><span class="sxs-lookup"><span data-stu-id="b980d-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="b980d-111">**Disabilitazione della notifica di benvenuto per i nuovi membri del gruppo di Office 365**</span><span class="sxs-lookup"><span data-stu-id="b980d-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="b980d-112">La notifica di benvenuto inviata agli utenti aggiunti ai gruppi di Office 365 può essere disabilitata impostando **UnifiedGroupWelcomeMessageEnabled** su False in Powershell.</span><span class="sxs-lookup"><span data-stu-id="b980d-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="b980d-113">Altre informazioni su questa impostazione [qui](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="b980d-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

