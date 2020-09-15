---
title: Un proprietario non può creare una sottocartella tramite Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 9590f780cffeaf644733752c763e04d748b1b39e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665722"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Un proprietario non può creare una sottocartella tramite Outlook

**È presente un problema ancora aperto con i proprietari delle cartelle pubbliche che creano sottocartelle usando Outlook. Il problema verrà risolto a breve.**

Nel frattempo, usare una delle soluzioni alternative seguenti:

1. Usare Outlook per MAC per creare la sottocartella poiché il problema riguarda solo Outlook desktop per Windows (tutte le versioni)
2. Chiedere a un amministratore di creare la sottocartella tramite Shell di Exchange Online o l'interfaccia di amministrazione di Exchange
3. Cambiare la DefaultPublicFolderMailbox/EffectivePublicFolderMailbox dell'utente in una cassetta postale diversa da quella del contenuto che causa il problema.  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. Attendere un'ora e riavviare il client di Outlook