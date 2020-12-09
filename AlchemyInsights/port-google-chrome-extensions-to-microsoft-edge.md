---
title: Porta Google Chrome Extensions to Microsoft Edge (cromo)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004032"
- "7102"
ms.openlocfilehash: 2a20f258cbcbca7c8db4e38c52464fefb1b6f39d
ms.sourcegitcommit: 38c87ed786dda7181562492d5d2e7ef0e18e0cab
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/08/2020
ms.locfileid: "49600149"
---
# <a name="port-google-chrome-extensions-to-microsoft-edge-chromium"></a><span data-ttu-id="6cdb2-102">Porta Google Chrome Extensions to Microsoft Edge (cromo)</span><span class="sxs-lookup"><span data-stu-id="6cdb2-102">Port Google Chrome extensions to Microsoft Edge (Chromium)</span></span>

<span data-ttu-id="6cdb2-103">È facile portare le [estensioni di Google Chrome a Microsoft Edge (cromo)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension).</span><span class="sxs-lookup"><span data-stu-id="6cdb2-103">It's easy to [port Google Chrome extensions to Microsoft Edge (Chromium)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension).</span></span> <span data-ttu-id="6cdb2-104">Nella maggior parte dei casi, sono necessarie solo modifiche minime per eseguire queste estensioni su Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="6cdb2-104">In most cases, only minimal changes are needed to run these extensions on Microsoft Edge.</span></span>

<span data-ttu-id="6cdb2-105">Le API di estensione e le chiavi dei manifesti supportate da Google Chrome sono compatibili con il codice Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="6cdb2-105">The extension APIs and manifest keys supported by Google Chrome are code-compatible with Microsoft Edge.</span></span> <span data-ttu-id="6cdb2-106">Tuttavia, Microsoft Edge non supporta le API di estensione Chrome. GCM, Chrome. Identity. getaccounts, Chrome. Identity. getAuthToken e Chrome. instanceID.</span><span class="sxs-lookup"><span data-stu-id="6cdb2-106">However, Microsoft Edge does not support the extension APIs chrome.gcm, chrome.identity.getAccounts, chrome.identity.getAuthToken, and chrome.instanceID.</span></span>