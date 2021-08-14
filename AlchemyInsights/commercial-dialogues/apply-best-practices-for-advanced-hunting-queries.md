---
title: Applicare le procedure consigliate per le query di ricerca avanzate
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: e2a22563a840cd6017afd343bad108be216738742938a48ba5ceb1010fd16098
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930137"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a>Applicare le procedure consigliate per le query di ricerca avanzate

Per ottenere risultati più veloci ed evitare timeout durante l'esecuzione di query complesse, applicare le procedure consigliate seguenti:

- Quando si provano nuove query, utilizzare sempre un limite per evitare di ottenere set di risultati estremamente grandi. Utilizzare inoltre `count` per effettuare una valutazione iniziale delle dimensioni del set di risultati.
- Usare prima i filtri del periodo. Idealmente, limitare le query a sette giorni.
- All'inizio di una query, subito dopo il filtro temporale, aggiungere i filtri previsti per rimuovere la maggior parte dei dati.
- Quando cerchi token completi, usa `has` l'operatore anziché `contains` .
- Eseguire una ricerca in una colonna specifica anziché in tutte le colonne.
- Quando si uniscono tabelle, specificare innanzitutto la tabella con un numero minore di righe.
- `project` solo le colonne necessarie delle tabelle unite.

Per ulteriori informazioni, vedere [Advanced hunting query best practices.](https://go.microsoft.com/fwlink/?linkid=2144812)
