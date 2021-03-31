---
title: Impostare Microsoft Edge come browser predefinito su un dispositivo macOS
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: 5318c7d20ee7091e162e566cd2b4ebf5d255915b
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426820"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-macos-device"></a><span data-ttu-id="1a316-102">Impostare Microsoft Edge come browser predefinito su un dispositivo macOS</span><span class="sxs-lookup"><span data-stu-id="1a316-102">Set Microsoft Edge as the default browser on a macOS device</span></span>

<span data-ttu-id="1a316-103">Usare uno dei due metodi seguenti per impostare Microsoft Edge come browser predefinito:</span><span class="sxs-lookup"><span data-stu-id="1a316-103">Use one of these two methods to set Microsoft Edge as the default browser:</span></span>

<span data-ttu-id="1a316-104">Metodo 1: eseguire il flashing del dispositivo con un'immagine macOS in cui Microsoft Edge sia già stato impostato come browser predefinito.</span><span class="sxs-lookup"><span data-stu-id="1a316-104">Method 1: Flash the device with an image of macOS where Microsoft Edge has already been set as the default browser.</span></span>

<span data-ttu-id="1a316-105">Metodo 2: impostare il criterio DefaultBrowserSettingEnabled per chiedere all'utente di impostare Microsoft Edge come browser predefinito.</span><span class="sxs-lookup"><span data-stu-id="1a316-105">Method 2: Set the DefaultBrowserSettingEnabled policy to prompt the user to set Microsoft Edge as the default browser.</span></span>

<span data-ttu-id="1a316-106">Entrambi i metodi consentono a un utente di cambiare il browser predefinito.</span><span class="sxs-lookup"><span data-stu-id="1a316-106">Either method allows a user to change the default browser.</span></span> <span data-ttu-id="1a316-107">Per questo motivo, si consiglia di implementare il criterio DefaultBrowserSettingEnabled anche con il metodo 1.</span><span class="sxs-lookup"><span data-stu-id="1a316-107">For this reason, we recommend that you deploy the DefaultBrowserSettingEnabled policy even if you used method 1.</span></span> <span data-ttu-id="1a316-108">Se un utente cambia il browser predefinito dopo aver implementato il criterio, quest'ultimo chiederà all'utente di reimpostare come browser predefinito Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="1a316-108">If a user changes the default browser after the policy is deployed, the policy prompts the user to set the default browser back to Microsoft Edge.</span></span>
