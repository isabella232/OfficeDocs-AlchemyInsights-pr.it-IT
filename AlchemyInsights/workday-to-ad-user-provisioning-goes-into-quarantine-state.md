---
title: Il provisioning utente di Workday in AD va nello stato quarantena
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8471"
- "9004687"
ms.openlocfilehash: 32a5d010b95b9587e121ca1526def743fd8f371b13d1d73d3578c692839edf19
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036496"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a>Il provisioning utente di Workday in AD va nello stato quarantena

**Il provisioning utente di Workday in AD va nello stato quarantena e non viene creato alcun utente in AD**

Il provisioning utente di Workday in AD è andato in stato quarantena e i registri di controllo mostrano eventi di esportazioni non andate a buon fine con il messaggio di errore **Errore: OperationsError-SvcErr: si è verificato un errore nell'operazione. Non è stato configurato alcun riferimento superiore per il servizio directory. Il servizio directory non è quindi in grado di generare riferimenti a oggetti che si trovano all'esterno di questa foresta.**. Questo errore in genere viene visualizzato se l'UO del contenitore di Active Directory non è impostata correttamente o se si sono verificati errori con il mapping espressione usato per **parentDistinguishedName**.

Controlla che l'UO predefinita per il parametro **Nuovi utenti** non contenga errori di digitazione. Assicurati che l'UO specificata esista già in AD. Se stai usando **parentDistinguishedName** nel mapping dell'attributo, assicurati che restituisca sempre un contenitore noto nel dominio AD. Verifica Esporta evento nei registri di controllo per visualizzare il valore generato.

Per altri dettagli sulla configurazione di Workday per il provisioning automatizzato, consulta [Tutorial: configurare Workday per il provisioning utente automatico](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).

