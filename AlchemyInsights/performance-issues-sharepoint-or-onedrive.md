---
title: Problemi relativi alle prestazioni-SharePoint o OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: aecbf4043c6456ece73f7deed6b068040f0691a2
ms.sourcegitcommit: 0fb89d8106fe409ab1b78e50f5357ffc2252f7c7
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/17/2019
ms.locfileid: "40068410"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint o OneDrive lento, inaccessibile o non disponibile per più utenti

SharePoint o OneDrive possono essere lenti, inaccessibili o non disponibili o possono visualizzare i servizi non disponibili o 503 errori, per diversi motivi:
  
- Se il sito di SharePoint o OneDrive è lento o ritardato per più utenti, potrebbe verificarsi un problema di servizio temporaneo in cui gli utenti avvertono ritardi intermittenti o errori di spostamento quando si accede a siti di SharePoint o di contenuto di OneDrive. Controllare il [Dashboard dell'integrità del servizio](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) per verificare se l'organizzazione ha un impatto.
  
- Gli utenti possono ricevere un *server 503 è* un errore durante il tentativo di accedere a siti di SharePoint o OneDrive. Questo errore può essere causato dalla limitazione all'interno del servizio di SharePoint. SharePoint Online utilizza la limitazione per mantenere le prestazioni ottimali e l'affidabilità del servizio SharePoint Online. La limitazione limita il numero di azioni utente o di chiamate simultanee (tramite script o codice) per impedire un utilizzo eccessivo delle risorse. Per ulteriori informazioni sulla limitazione, vedere [impedire la limitazione o il blocco in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

- Se si verifica un rallentamento delle prestazioni con un sito o una pagina di SharePoint **classica** o **moderna** , utilizzare lo [strumento di diagnostica della pagina](https://aka.ms/perftool) per analizzare le pagine.
  
- Se si verificano ancora prestazioni generali lente, vedere le risorse nella parte inferiore di questo articolo: [Introduzione all'ottimizzazione delle prestazioni per SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)
  