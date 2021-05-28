---
title: Registrazione delle chiamate 1:1
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "7648"
ms.openlocfilehash: 18c68fee514681b2a81c3cfa022c29ce83834f22
ms.sourcegitcommit: 610a5d950cdf488870601762ef52d881e3e22a48
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/28/2021
ms.locfileid: "52696962"
---
# <a name="11-call-recording"></a><span data-ttu-id="edf39-102">Registrazione delle chiamate 1:1</span><span class="sxs-lookup"><span data-stu-id="edf39-102">1:1 call recording</span></span>

<span data-ttu-id="edf39-103">Se il **pulsante Avvia** registrazione è disattivato in una chiamata 1:1, è necessario modificare le impostazioni dei criteri per l'utente che ha subito l'impatto.</span><span class="sxs-lookup"><span data-stu-id="edf39-103">If the **Start Recording** button is grayed out in a 1:1 call, you need to change the policy settings for the impacted user.</span></span>   

<span data-ttu-id="edf39-104">A partire dal 31 maggio 2021, inizieremo a far rispettare un nuovo Teams criteri di chiamata *AllowCloudRecordingForCalls.*</span><span class="sxs-lookup"><span data-stu-id="edf39-104">Beginning May 31, 2021, we'll start enforcing a new Teams Calling Policy *AllowCloudRecordingForCalls*.</span></span> <span data-ttu-id="edf39-105">Prima di questa modifica, la registrazione delle chiamate 1:1 è controllata dal criterio *AllowCloudRecording* Teams Riunione.</span><span class="sxs-lookup"><span data-stu-id="edf39-105">Prior to this change, 1:1 call recording is controlled by the *AllowCloudRecording* Teams Meeting Policy.</span></span> <span data-ttu-id="edf39-106">Questa modifica è documentata nel post del Centro messaggi: [(Aggiornato) 1:1 Introduzione ai](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)criteri di registrazione delle chiamate .</span><span class="sxs-lookup"><span data-stu-id="edf39-106">This change is documented in the Message Center post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).</span></span>  

<span data-ttu-id="edf39-107">*AllowCloudRecordingForCalls*   l'opzione dei criteri di chiamata è **$False** per impostazione predefinita.</span><span class="sxs-lookup"><span data-stu-id="edf39-107">*AllowCloudRecordingForCalls* calling policy option is set to **$False** by default.</span></span> <span data-ttu-id="edf39-108">Se si preferisce impedire a tutti gli utenti di registrare chiamate 1:1, non è necessario eseguire alcuna azione.</span><span class="sxs-lookup"><span data-stu-id="edf39-108">If you prefer to block all users from recording 1:1 calls, you don't need to take any action.</span></span>  

<span data-ttu-id="edf39-109">Per abilitare la registrazione delle chiamate per tutti gli utenti nelle chiamate 1:1, utilizzare Teams PowerShell per eseguire il cmdlet seguente:</span><span class="sxs-lookup"><span data-stu-id="edf39-109">To enable call recording for all users in 1:1 calls use Teams PowerShell to run the following cmdlet:</span></span> 

<span data-ttu-id="edf39-110">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span><span class="sxs-lookup"><span data-stu-id="edf39-110">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span></span> 

<span data-ttu-id="edf39-111">In alternativa, puoi creare un nuovo criterio e impostare **-AllowCloudRecordingForCalls** su **$true** e assegnare tale criterio agli utenti.</span><span class="sxs-lookup"><span data-stu-id="edf39-111">Alternatively, you can create a new policy and set **-AllowCloudRecordingForCalls** to **$true** and assign that policy to your users.</span></span> 

<span data-ttu-id="edf39-112">Per ulteriori informazioni, vedere [1:1 Call Recording Policy Controls Are (Almost!) Qui](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span><span class="sxs-lookup"><span data-stu-id="edf39-112">For more information, see [1:1 Call Recording Policy Controls Are (Almost!) Here](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span></span>
