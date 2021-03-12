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
ms.openlocfilehash: af09e8805409446a42a62c82aa577ad27f09a17a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50733853"
---
# <a name="11-call-recording"></a><span data-ttu-id="44599-102">Registrazione delle chiamate 1:1</span><span class="sxs-lookup"><span data-stu-id="44599-102">1:1 call recording</span></span>

<span data-ttu-id="44599-103">Gli amministratori devono intervenire ora per continuare a consentire agli utenti di registrare le chiamate 1:1.</span><span class="sxs-lookup"><span data-stu-id="44599-103">Administrators need to take action now to continue allowing users to Record 1:1 calls.</span></span>
 
<span data-ttu-id="44599-104">A partire dal 12 aprile 2021, inizieremo ad applicazione di una nuova opzione dei criteri di chiamata di Teams *AllowCloudRecordingForCalls.*</span><span class="sxs-lookup"><span data-stu-id="44599-104">Beginning April 12, 2021, we will start enforcing a new Teams Calling Policy option *AllowCloudRecordingForCalls*.</span></span> 

<span data-ttu-id="44599-105">Attualmente le funzionalità di registrazione delle chiamate 1:1 sono controllate dall'opzione *AllowCloudRecording* in Criteri riunione di Teams.</span><span class="sxs-lookup"><span data-stu-id="44599-105">Currently 1:1 call recording capabilities are controlled by the *AllowCloudRecording* option in Teams Meeting Policies.</span></span> <span data-ttu-id="44599-106">Se gli utenti sono autorizzati a registrare riunioni di Teams, possono anche registrare chiamate 1:1.</span><span class="sxs-lookup"><span data-stu-id="44599-106">If your users are allowed to record Teams Meetings they can also record 1:1 calls.</span></span>

<span data-ttu-id="44599-107">Se si preferisce impedire a tutti gli utenti di registrare chiamate 1:1, non è necessario eseguire alcuna azione.</span><span class="sxs-lookup"><span data-stu-id="44599-107">If you prefer to block all users from recording 1:1 calls, you do not need to take any action.</span></span> <span data-ttu-id="44599-108">L'opzione del criterio di chiamata *AllowCloudRecordingForCalls* $False per impostazione predefinita.</span><span class="sxs-lookup"><span data-stu-id="44599-108">*AllowCloudRecordingForCalls* calling policy option will be $False by default.</span></span>

<span data-ttu-id="44599-109">Questa modifica è documentata nel post del Centro messaggi seguente: (Aggiornato) Introduzione ai criteri di registrazione delle chiamate [1:1](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) Per impostare l'opzione Criteri di chiamata di Teams, è necessario utilizzare [Teams PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-install)</span><span class="sxs-lookup"><span data-stu-id="44599-109">This change is documented in the following Message Center Post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) To set the Teams Calling Policy Option you must use [Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install).</span></span>

<span data-ttu-id="44599-110">Per abilitare la registrazione delle chiamate nelle chiamate **1:1:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True</span><span class="sxs-lookup"><span data-stu-id="44599-110">**To enable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True</span></span>

<span data-ttu-id="44599-111">**Per disabilitare la registrazione delle chiamate in chiamate 1:1:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False</span><span class="sxs-lookup"><span data-stu-id="44599-111">**To disable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False</span></span>

