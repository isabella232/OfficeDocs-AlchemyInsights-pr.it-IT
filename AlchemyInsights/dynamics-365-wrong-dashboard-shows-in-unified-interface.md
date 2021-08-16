---
title: Dynamics 365 - Dashboard errato mostra nell'interfaccia unificata di Dynamics 365
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 1edb2a7e9e0c270c7e98eb43d2f6514d70c39a19ea97d189322ca387b6842a18
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101486"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Dashboard errato nell'interfaccia unificata di Dynamics 365

Esistono diversi motivi per cui è possibile visualizzare un dashboard diverso da quello previsto:

## <a name="the-user-has-set-a-user-default-dashboard"></a>L'utente ha impostato un dashboard predefinito dell'utente 

In genere è possibile identificare l'impostazione di un dashboard predefinito dell'utente se il pulsante Imposta come predefinito non viene visualizzato nella barra dei comandi del dashboard.  Il dashboard predefinito dell'utente sostituisce tutti gli altri dashboard predefiniti, anche se il dashboard predefinito dell'utente non è presente nell'app corrente.

Utilizzare la soluzione alternativa seguente per annullare l'impostazione del dashboard predefinito.

1. Creare un nuovo dashboard personale.

2. Imposta il nuovo dashboard come predefinito dell'utente.

3. Eliminare il dashboard.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Il dashboard viene impostato nella mappa del sito

Potresti aver impostato un dashboard predefinito dell'organizzazione selezionando un dashboard e scegliendo "Imposta come predefinito" in "Personalizza il sistema". Tuttavia, il dashboard definito nel progettista della mappa del sito avrà la precedenza su questo dashboard, se l'utente ha accesso ad esso.

Per fare in modo che gli utenti vedano il dashboard impostato come predefinito dell'organizzazione, è possibile:

* Impostare il dashboard nella mappa del sito

* Rimuovere l'accesso al dashboard definito per la mappa del sito per tali utenti
