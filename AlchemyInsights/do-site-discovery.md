---
title: Eseguire l'individuazione dei siti
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9143"
- "9005291"
ms.openlocfilehash: bdf94220de45d92f63e56501ea4e35389224d25c
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 03/08/2021
ms.locfileid: "50529313"
---
# <a name="do-site-discovery"></a>Eseguire l'individuazione dei siti

Se l'organizzazione usa ancora versioni legacy di applicazioni e piani Web e si prevede di utilizzare la modalità Internet Explorer, come la maggior parte dei clienti, occorre eseguire un'ulteriore individuazione dei siti.

**È già stata distribuita una versione precedente di Microsoft Edge**

Se è già stato configurato l'elenco dei siti modalità Enterprise in modo che funzioni per la versione legacy di Microsoft Edge, l'individuazione dei siti è quasi completata. L'unica cosa che occorre fare è aggiungere siti neutri.

In genere i siti neutri sono siti che forniscono Single Sign-On (SSO). Se si passa a un sito neutro da Microsoft Edge, è possibile usare Microsoft Edge per eseguire l'autenticazione. Se si passa a un sito neutro in modalità Internet Explorer, è possibile usare la modalità Internet Explorer per eseguire l'autenticazione.

Identificare tutti i siti SSO o altri siti neutri utilizzati e aggiungerli all'elenco dei siti modalità Enterprise.

**Internet Explorer è il browser predefinito**.

Se si usa solo Internet Explorer, è probabile che non si sappia quali siti sono stati aggiornati agli standard Web moderni e richiedono ancora Internet Explorer. È possibile trovare e aggiungere questi siti all'elenco dei siti modalità Enterprise in modo da poter usare la modalità Internet Explorer solo per tali siti.

> [!NOTE]
> [Individuazione di siti modalità Enterprise](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery): individua i siti che potrebbero richiedere la modalità Internet Explorer. È possibile raccogliere dati nei computer che eseguono Windows Internet Explorer 8 tramite Internet Explorer 11 in Windows 10, Windows 8.1 o Windows 7.

**Analisi dei dati**.

Dopo aver raccolto i dati del sito, per analizzare i dati è consigliabile eseguire il processo in 4 passaggi riportato di seguito:
1. Ordinare i dati in base al dominio, quindi in base all'URL.
2. Definire i limiti di un'app da configurare per la modalità Internet Explorer. È possibile includere tutti i siti e i controlli Web che definiscono l'app, ma non è possibile includere altri siti e controlli. Alcuni siti possono essere semplici, ad esempio *https://contoso.com/app1*, mentre altri possono richiedere la definizione di più siti e pagine.
3. Eseguire un test dell'app per verificare che non funzioni in modo nativo. Molti siti offriranno contenuti moderni quando rilevano un browser moderno e solo contenuti legacy quando individuano Internet Explorer.
4. Aggiungere l'app all'elenco dei siti modalità Enterprise se non si riesce a eseguire il test.

> [!NOTE]
> Come procedura consigliata, raggruppare tutti i siti che comprendono un'app. In questo modo, quando si aggiorna un'app, è più facile rimuovere l'intero sito dalla modalità Internet Explorer e iniziare a usare un browser moderno per l'app specifica.

Dopo aver completato l'individuazione dei siti e aver analizzato i dati, è possibile iniziare a considerare la strategia del canale.

