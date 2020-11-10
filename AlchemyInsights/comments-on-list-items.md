---
title: Commenti sugli elementi di elenco
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003821"
- "6841"
ms.openlocfilehash: 5940d1a96324c5ca77331485a115689abe547ef7
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/09/2020
ms.locfileid: "48947507"
---
# <a name="comments-on-list-items"></a>Commenti sugli elementi di elenco

Gli utenti saranno presto in grado di aggiungere ed eliminare commenti sugli elementi dell'elenco. Gli utenti possono visualizzare tutti i commenti su un elemento di elenco e filtrare tra le visualizzazioni che mostrano commenti o attività correlate a un elemento.

**Tempistica** :

**Rilascio mirato** : distribuzione graduale a metà ottobre e prevista per il completamento entro la metà di novembre

**Standard Release** : graduale roll out a metà novembre e previsto per il completamento entro l'inizio di dicembre

**Implementazione** : rilascio mirato per l'intera organizzazione

Gli utenti devono tenere presente quanto segue prima di poter aggiungere ed eliminare commenti:

- I commenti seguono le impostazioni di autorizzazione inerenti a SharePoint.
- Gli elenchi classici che non sono ancora stati creati per essere visualizzati nelle interfacce utente moderne, come gli elenchi di attività, non avranno questa funzionalità di commento.
- La creazione di commenti negli elenchi dei team non è disponibile con questa versione.
- I commenti non vengono indicizzati dalla ricerca.

Gli amministratori possono disabilitare questa funzionalità a livello di organizzazione modificando il parametro **CommentsOnListItemsDisabled** nel cmdlet **set-SPOTenant** di PowerShell.

Al momento non è possibile disabilitare il commento a livello di sito o di elenco. Si spera di disporre di tali controlli in un aggiornamento successivo, probabilmente nel primo trimestre 2021.
