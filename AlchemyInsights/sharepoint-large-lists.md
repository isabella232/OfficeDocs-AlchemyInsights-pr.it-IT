---
title: Elenchi di grandi dimensioni di SharePoint
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 2/12/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: 222ad554de0d94dcfd4e34e9a2c6aa8ab4e6f81f
ms.sourcegitcommit: d7e1b097d3866782f508527c797426dc56c6ba17
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 10/14/2019
ms.locfileid: "37488521"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a>Utilizzo di elenchi e raccolte di grandi dimensioni in SharePoint

Gli elenchi e le raccolte di SharePoint possono contenere fino a 30 milioni elementi, ma quando dispongono di più di 5.000 elementi, è possibile che venga visualizzato un errore di soglia per la visualizzazione elenco quando si tenta di utilizzarli. Questa soglia è in atto per mantenere le prestazioni del servizio. Non è possibile modificarlo. Per evitare di colpire questa soglia:

**USA moderna**

Le visualizzazioni che mostrano molti elementi funzionano meglio nell'esperienza moderna. [Utilizzare l'esperienza moderna](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) per evitare errori che potrebbero essere visualizzati nell'esperienza classica.

**Aggiungere indici**

Quando si filtra o si ordina in base a una colonna che non dispone di un indice, è possibile che venga visualizzato un messaggio di errore. [Aggiungere un indice](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manualmente dalle **impostazioni dell'elenco** nel menu impostazioni, quindi **colonne indicizzate**.

**Modificare la visualizzazione elenco**

Se si verifica un errore durante l'utilizzo di un elenco di grandi dimensioni, [modificare la visualizzazione elenco](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).

Le quattro modifiche seguenti elimineranno gli errori di soglia della visualizzazione elenco. Apportare tutte e quattro le modifiche per rimuovere tutti gli errori. Se si verificano ancora errori, controllare la [gestione di elenchi e raccolte di grandi dimensioni](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).

1. Selezionare **None** dal **primo ordinamento in base alla colonna** e **quindi ordinare in base alla colonna**.
2. Selezionare **None** dal **primo gruppo in base alla colonna** e **quindi raggruppare in base alla colonna**.
3. Selezionare **Nessuna** per tutte le colonne nella sezione **totali** .
4. Deselezionare tutte le colonne, tranne una per la visualizzazione, dalla sezione **Columns** .

