---
title: Il grafico mostra un numero diverso di record nella griglia
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5611"
- "9002930"
ms.openlocfilehash: 68ba6caf602a5cf60e2c96c80703f19dd07c3b6430c2a66f40fea4a2f3d06e75
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53950084"
---
# <a name="chart-shows-different-number-of-records-in-grid"></a>Il grafico mostra un numero diverso di record nella griglia

**Sintomo**

Per il grafico nella pagina del dashboard, quando si fa clic sul grafico "..." e su "Visualizza record", si passa alla pagina della griglia per visualizzare tutti i record. A volte il numero di record cambia.

**Causa**

Ciò è dovuto alle diverse visualizzazioni tra il grafico nella pagina del dashboard originale e il grafico nella griglia della home page.  

**Soluzione**

1. Controllare la visualizzazione dalla pagina originale e quella nella griglia per vedere se sono diverse.
2. Cambiare la visualizzazione nella griglia in modo che corrisponda alla visualizzazione nella pagina originale.
3. Se non è possibile trovare la visualizzazione corretta, in genere significa che la visualizzazione non è abilitata nella progettazione app.
4. Passare alla progettazione app dell'app specifica, scegliere l'entità e le relative visualizzazioni, selezionare la visualizzazione che si desidera abilitare, salvare, pubblicare e chiudere.
5. Aggiornare la pagina.