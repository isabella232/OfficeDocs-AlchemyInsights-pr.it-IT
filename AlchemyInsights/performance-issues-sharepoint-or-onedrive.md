---
title: Problemi relativi alle prestazioni-SharePoint o OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 28867b71df5353dcee5cc3361742f10357a0efe1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771905"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint o OneDrive lento, inaccessibile o non disponibile per più utenti

SharePoint o OneDrive possono essere lenti, inaccessibili o non disponibili o possono visualizzare i servizi non disponibili o 503 errori, per diversi motivi:
  
- Se il sito di SharePoint o OneDrive è lento o ritardato per più utenti, potrebbe verificarsi un problema di servizio temporaneo in cui gli utenti avvertono ritardi intermittenti o errori di spostamento quando si accede a siti di SharePoint o di contenuto di OneDrive. Controllare il [dashboard sull'integrità dei servizi](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) per verificare se l'organizzazione è interessata.
  
- Gli utenti possono ricevere un *server 503 è* un errore durante il tentativo di accedere a siti di SharePoint o OneDrive. Questo errore può essere causato dalla limitazione all'interno del servizio di SharePoint. SharePoint Online usa la limitazione per garantire prestazioni e affidabilità ottimali del servizio SharePoint Online. La limitazione limita il numero delle azioni dell'utente o delle chiamate simultanee (in base al codice o script) per evitare il consumo eccessivo di risorse. Per ulteriori informazioni sulla limitazione, vedere [impedire la limitazione o il blocco in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

- Se si verifica un rallentamento delle prestazioni con un sito o una pagina di SharePoint **classica** o **moderna** , utilizzare lo [strumento di diagnostica della pagina](https://aka.ms/perftool) per analizzare le pagine.
  
- Se si verificano ancora prestazioni generali lente, vedere le risorse nella parte inferiore di questo articolo: [Introduzione all'ottimizzazione delle prestazioni per SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)
  