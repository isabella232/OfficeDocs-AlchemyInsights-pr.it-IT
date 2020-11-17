---
title: Creare un gruppo
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
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086391"
---
# <a name="create-a-group"></a><span data-ttu-id="33854-102">Creare un gruppo</span><span class="sxs-lookup"><span data-stu-id="33854-102">Create a group</span></span>

<span data-ttu-id="33854-103">In questo argomento viene descritta la creazione di gruppi.</span><span class="sxs-lookup"><span data-stu-id="33854-103">This topic describes group creation.</span></span>

<span data-ttu-id="33854-104">**Autorizzazione per la creazione di un gruppo**</span><span class="sxs-lookup"><span data-stu-id="33854-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="33854-105">Assicurarsi di essere autorizzati a creare un nuovo gruppo.</span><span class="sxs-lookup"><span data-stu-id="33854-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="33854-106">Gli amministratori globali possono disabilitare la creazione del gruppo nel portale di Azure o nel pannello di accesso.</span><span class="sxs-lookup"><span data-stu-id="33854-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="33854-107">Potrebbe essere necessario un amministratore per creare il nuovo gruppo o per fornire le autorizzazioni appropriate.</span><span class="sxs-lookup"><span data-stu-id="33854-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="33854-108">**Gestire le autorizzazioni per la creazione di gruppi**</span><span class="sxs-lookup"><span data-stu-id="33854-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="33854-109">Gli amministratori globali possono gestire le autorizzazioni per la creazione di gruppi (per motivi relativi alla sicurezza) o i gruppi di Office 365 creati nel portale di Azure o nel pannello di accesso, scegliendo "gli utenti possono creare gruppi di sicurezza nei portali di Azure" o "gli utenti possono creare gruppi di Office 365 nei portali di Azure" in **tutti i gruppi**  >  **generale (impostazioni)**.</span><span class="sxs-lookup"><span data-stu-id="33854-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="33854-110">È inoltre possibile limitare la creazione di gruppi per selezionare un gruppo di utenti se si dispone di una licenza di Azure Active Directory P1 Premium.</span><span class="sxs-lookup"><span data-stu-id="33854-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="33854-111">**Disabilitazione della notifica di benvenuto per i nuovi membri del gruppo di Office 365**</span><span class="sxs-lookup"><span data-stu-id="33854-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="33854-112">La notifica di benvenuto inviata agli utenti che sono stati aggiunti ai gruppi di Office 365 può essere disattivata impostando **UnifiedGroupWelcomeMessageEnabled** su false in PowerShell.</span><span class="sxs-lookup"><span data-stu-id="33854-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="33854-113">Per ulteriori informazioni su [questa impostazione,](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)vedere.</span><span class="sxs-lookup"><span data-stu-id="33854-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

