---
title: Un proprietario non può creare una sottocartella tramite Outlook
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: b2ab7b60bc521fd28d68333bb963528f7b9e05f2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836139"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Un proprietario non può creare una sottocartella tramite Outlook

**È presente un problema ancora aperto con i proprietari delle cartelle pubbliche che creano sottocartelle usando Outlook. Il problema verrà risolto a breve.**

Nel frattempo, usare una delle soluzioni alternative seguenti:

1. Usare Outlook per MAC per creare la sottocartella poiché il problema riguarda solo Outlook desktop per Windows (tutte le versioni)
2. Chiedere a un amministratore di creare la sottocartella tramite Shell di Exchange Online o l'interfaccia di amministrazione di Exchange
3. Cambiare la DefaultPublicFolderMailbox/EffectivePublicFolderMailbox dell'utente in una cassetta postale diversa da quella del contenuto che causa il problema.  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. Attendere un'ora e riavviare il client di Outlook