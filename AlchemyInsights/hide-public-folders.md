---
title: Nascondere le cartelle pubbliche
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "8417"
ms.openlocfilehash: 70179296e9c1bb7391535f55796bc5af80b825f8
ms.sourcegitcommit: a019bd8b0244914edb59e124bc6538cdc5c158f9
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 02/18/2021
ms.locfileid: "50294643"
---
# <a name="hide-public-folders"></a><span data-ttu-id="da0ab-102">Nascondere le cartelle pubbliche</span><span class="sxs-lookup"><span data-stu-id="da0ab-102">Hide public folders</span></span>

<span data-ttu-id="da0ab-103">**Nascondere l'intero albero delle cartelle pubbliche**:</span><span class="sxs-lookup"><span data-stu-id="da0ab-103">**To hide entire public folder tree**:</span></span>

<span data-ttu-id="da0ab-104">Usare i passaggi descritti in [questo](https://aka.ms/ControlPF) articolo per nascondere l'intero albero delle cartelle pubbliche da utenti selezionati o da tutti gli utenti.</span><span class="sxs-lookup"><span data-stu-id="da0ab-104">Use the steps in [this](https://aka.ms/ControlPF) article to hide entire public folder tree from selective or all users.</span></span>

<span data-ttu-id="da0ab-105">**Nascondere una specifica cartella pubblica**:</span><span class="sxs-lookup"><span data-stu-id="da0ab-105">**To hide a specific public folder**:</span></span>

1. <span data-ttu-id="da0ab-106">Aggiungere le autorizzazioni per gli utenti che devono accedere alla cartella pubblica</span><span class="sxs-lookup"><span data-stu-id="da0ab-106">Add permissions for users who need to access the public folder</span></span>

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. <span data-ttu-id="da0ab-107">Rimuovere l'utente **predefinito** dall'**elenco** delle autorizzazioni:</span><span class="sxs-lookup"><span data-stu-id="da0ab-107">Remove the user **Default** from the **permission** list:</span></span>

    `Remove-PublicFolderClientPermission \test1 -User Default`
