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
ms.openlocfilehash: 66c76947d553c32475ebe7a11e69246b5b3a2882bb3d022873d85b93b3e87887
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53945746"
---
# <a name="hide-public-folders"></a>Nascondere le cartelle pubbliche

**Nascondere l'intero albero delle cartelle pubbliche**:

Usare i passaggi descritti in [questo](https://aka.ms/ControlPF) articolo per nascondere l'intero albero delle cartelle pubbliche da utenti selezionati o da tutti gli utenti.

**Nascondere una specifica cartella pubblica**:

1. Aggiungere le autorizzazioni per gli utenti che devono accedere alla cartella pubblica

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. Rimuovere l'utente **predefinito** dall'**elenco** delle autorizzazioni:

    `Remove-PublicFolderClientPermission \test1 -User Default`
