---
title: Problema con l'attributo e il filtro di ambito
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
- "8470"
- "9004687"
ms.openlocfilehash: 51ed0fabe220d0069d721ec64d049787bacd5b094e19f0c1996a28e07bb56f03
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960191"
---
# <a name="problem-with-attribute-and-scoping-filter"></a>Problema con l'attributo e il filtro di ambito

**Problema con valori UPN in conflitto**

Il provisioning utenti da Workday ad AD restituisce il messaggio di errore **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**. L'operazione non è riuscita perché il valore UPN fornito per l'aggiunta o la modifica non è univoco a livello di foresta. Dettagli errore: **CONSTRAINT_ATT_TYPE - userPrincipalName**.

Il valore **userPrincipalName** che il connettore Workday sta provando a impostare durante la creazione l'account utente di AD esiste già nel dominio Active Directory di destinazione. Ciò significa che (1) l'utente esiste già e il controllo degli ID corrispondenti non è riuscito oppure (2) la regola di generazione UPN ha generato un valore in conflitto.

Ecco la procedura di risoluzione suggerita:

Se l'utente esiste già e il controllo degli ID corrispondenti non è riuscito a collegare l'account Workday all'account Active Directory, verificare se l'attributo ID corrispondente ( in genere **employeeID**) sia in Workday che AD abbia una corrispondenza esatta. Se non hanno corrispondenze, occorre risolvere un problema relativo ai dati. Ad esempio, se l'EmployeeID in Workday è 001052 e in Active Directory è 1052, il motore di provisioning non riuscirà a collegare i due account e tenterà di creare un utente già esistente. La soluzione in questo caso consiste nel modificare il valore di **EmployeeID** in Active Directory in modo da includere gli zeri iniziali per impostarlo come 001052.
Se l'espressione che genera l'UPN non genera un valore univoco, è consigliabile usare la funzione di deduplicazione **SelectUniqueValue** per generare un valore univoco ogni volta.

**Il provisioning utente da Workday ad AD non imposta il valore dell'attributo manager per l'account utente di AD**

Il provisioning utenti da Workday ad AD non imposta il valore dell'attributo **manager** per gli account utente di AD. Questo comportamento può essere visualizzato in due scenari:

1. Il manager in Workday non può essere risolto in un account utente di AD corrispondente perché il manager non è nell'ambito.
2. In uno scenario **più domini AD**, il manager in Workday non è presente nello stesso dominio dell'utente.

Provare questa procedura per risolvere il problema:

1. Se sono stati definiti filtri di ambito, verificare prima di tutto che il manager sia nell'ambito e che soddisfi la clausola di ambito. Se il manager non soddisfa il filtro di ambito, modificare il filtro in modo che anche il responsabile sia nell'ambito dell'operazione di provisioning.
2. Se si hanno più domini Active Directory, il connettore presenta una limitazione nota di impossibilità a risolvere i riferimenti di manager tra domini.

Per altri dettagli sulla configurazione di Workday per il provisioning automatizzato, vedere [Tutorial: configurare Workday per il provisioning utente automatico](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).













