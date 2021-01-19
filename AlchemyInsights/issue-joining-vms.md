---
title: Problemi nell'aggiunta di macchine virtuali
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7924"
- "9004395"
ms.openlocfilehash: 77a889f05d6c4e7b19a1e0a66a99ffc0565c69d8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884585"
---
# <a name="issue-joining-vms"></a>Problemi nell'aggiunta di macchine virtuali

Per risolvere eventuali problemi che si verificano quando si cerca di aggiungere delle macchine virtuali, seguire questi passaggi:

1. Provare ad accedere usando il formato **UPN** (ad esempio, 'joeuser@contoso.com') al posto del formato **SAMAccountName** ('CONTOSO\joeuser').
2. Verificare di aver abilitato la sincronizzazione tramite password in conformità ai passaggi indicati nella *Guida introduttiva*.
3. Verificare che l'account utente interessato non sia un account esterno nel tenant Azure AD. Gli utenti esterni non possono accedere al dominio gestito dato che Azure AD Domain Services non dispone delle credenziali di tali account utente.
4. Se l'account utente interessato è un account utente solo cloud, verificare che gli utenti abbiano modificato la loro password dopo aver abilitato Azure Active Directory Domain Services. Questo passaggio porta alla generazione degli hash delle credenziali per Azure AD Domain Services.
5. Se gli account utente interessati vengono sincronizzati da una directory locale, verificare che sia stata configurata la release consigliata di Azure AD Connect per eseguire una sincronizzazione completa.
6. Se, dopo aver eseguito il Passaggio 4, i problemi dovessero persistere, eseguire i seguenti comandi dal computer di sincronizzazione:
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     `"net start 'Microsoft Azure AD Sync'"`.