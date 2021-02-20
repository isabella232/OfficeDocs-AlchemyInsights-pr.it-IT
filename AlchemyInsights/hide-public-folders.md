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
# <a name="hide-public-folders"></a>Nascondere le cartelle pubbliche

**Nascondere l'intero albero delle cartelle pubbliche**:

Usare i passaggi descritti in [questo](https://aka.ms/ControlPF) articolo per nascondere l'intero albero delle cartelle pubbliche da utenti selezionati o da tutti gli utenti.

**Nascondere una specifica cartella pubblica**:

1. Aggiungere le autorizzazioni per gli utenti che devono accedere alla cartella pubblica

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. Rimuovere l'utente **predefinito** dall'**elenco** delle autorizzazioni:

    `Remove-PublicFolderClientPermission \test1 -User Default`
