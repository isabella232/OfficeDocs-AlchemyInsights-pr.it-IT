---
title: SharePoint elenchi di grandi dimensioni
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: c67632e323f2068faba06779b94ba4fd8e9f319e18cefb7977bd3038ca770210
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53941605"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a>Utilizzare elenchi e raccolte di grandi dimensioni in SharePoint

SharePoint elenchi e raccolte possono contenere fino a 30 milioni di elementi, ma quando hanno più di 5.000 elementi, è possibile che venga visualizzato un errore Soglia visualizzazione elenco quando si tenta di lavorarvi. Questa soglia è pensata per garantire le prestazioni del servizio e non può essere modificata. Per evitare di raggiungere questa soglia:

**Usa moderno**

Le visualizzazioni che mostrano molti elementi funzionano meglio nell'esperienza moderna. [Usa l'esperienza moderna](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) per evitare errori che potresti visualizzare nell'esperienza classica.

**Aggiungere indici**

Quando si filtra o si ordina in base a una colonna che non dispone di un indice, è possibile che venga visualizzato un messaggio di errore. [Aggiungere manualmente un](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) indice da **List Impostazioni** nel menu delle impostazioni, quindi **Indexed Columns.**

**Modificare la visualizzazione elenco**

Se si verifica un errore quando si utilizza un elenco di grandi dimensioni, [modificare la visualizzazione elenco.](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372)

Le quattro modifiche seguenti rimuoveranno gli errori di soglia della visualizzazione elenco. Apportare tutte e quattro le modifiche per rimuovere tutti gli errori. Se si verificano ancora errori, selezionare [Gestisci elenchi e raccolte di grandi dimensioni.](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59)

1. Selezionare **Nessuno da** Primo **ordinamento in base alla colonna** e Quindi **ordinare in base alla colonna.**
2. Selezionare **Nessuno dal** primo gruppo in base alla **colonna** e **quindi raggruppare in base alla colonna.**
3. Selezionare **Nessuna per** tutte le colonne nella **sezione** Totali.
4. Deseleziona tutte le colonne ad una sola per la visualizzazione dalla **sezione** Colonne.

