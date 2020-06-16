---
title: Un proprietario non può creare una sottocartella tramite Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 2116bb837e4378ea29d7882df1d3010b3a4e0b1c
ms.sourcegitcommit: 936330b11fec49f6174eadea6c765bdf9e6ba784
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 06/12/2020
ms.locfileid: "44716600"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Un proprietario non può creare una sottocartella tramite Outlook

**È presente un problema ancora aperto con i proprietari delle cartelle pubbliche che creano sottocartelle usando Outlook. Il problema verrà risolto a breve.**

Nel frattempo, usare una delle soluzioni alternative seguenti:

1. Usare Outlook per MAC per creare la sottocartella poiché il problema riguarda solo Outlook desktop per Windows (tutte le versioni)
2. Chiedere a un amministratore di creare la sottocartella tramite Shell di Exchange Online o l'interfaccia di amministrazione di Exchange
3. Cambiare la DefaultPublicFolderMailbox/EffectivePublicFolderMailbox dell'utente in una cassetta postale diversa da quella del contenuto che causa il problema.  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. Attendere un'ora e riavviare il client di Outlook