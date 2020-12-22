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
ms.openlocfilehash: 2ee95e98aae3d9ec9a933f9cae234111d4285edd
ms.sourcegitcommit: 2eb1dd0856509b9907ccba9a5cb99d09b4f6eb4b
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/21/2020
ms.locfileid: "49724158"
---
# <a name="comments-on-list-items"></a>Commenti sugli elementi di elenco

Gli utenti possono visualizzare tutti i commenti su un elemento di elenco e filtrare tra le visualizzazioni che mostrano commenti o attività correlate a un elemento.

Gli utenti devono tenere presente quanto segue prima di poter aggiungere ed eliminare commenti:

- I commenti seguono le impostazioni di autorizzazione inerenti a SharePoint.
- Gli elenchi classici che non sono ancora stati creati per essere visualizzati nelle interfacce utente moderne, come gli elenchi di attività, non avranno questa funzionalità di commento.
- La creazione di commenti negli elenchi dei team non è disponibile con questa versione.
- I commenti non vengono indicizzati dalla ricerca.

Gli amministratori possono disabilitare questa funzionalità a livello di organizzazione modificando il parametro **CommentsOnListItemsDisabled** nel cmdlet **set-SPOTenant** di PowerShell.

Al momento non è possibile disabilitare il commento a livello di sito o di elenco. Si spera di disporre di tali controlli in un aggiornamento successivo, probabilmente nel primo trimestre 2021.
