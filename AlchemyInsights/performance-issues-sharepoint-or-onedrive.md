---
title: Problemi di prestazioni SharePoint o OneDrive
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
ms.openlocfilehash: 921aae7eba8487c5600f290fd671ef2675372e6af0478b913e38354856cbaa22
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53911846"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint o OneDrive lento, inaccessibile o non disponibile per più utenti

SharePoint o OneDrive potrebbe essere lento, inaccessibile o non disponibile oppure potrebbe essere visualizzato un servizio non disponibile o errori 503, per diversi motivi:
  
- Se il sito di SharePoint o OneDrive è lento o ritardato per più utenti, potrebbe verificarsi un problema di servizio temporaneo in cui gli utenti si verificano ritardi intermittenti o errori di spostamento durante l'accesso a siti di SharePoint o OneDrive contenuto. Controllare il [dashboard sull'integrità dei servizi](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) per verificare se l'organizzazione è interessata.
  
- Gli utenti potrebbero ricevere un *errore 503 server* occupato quando si tenta di accedere a SharePoint o OneDrive siti. Questo errore può essere causato dalla limitazione all'interno del SharePoint servizio. SharePoint Online usa la limitazione per garantire prestazioni e affidabilità ottimali del servizio SharePoint Online. La limitazione limita il numero delle azioni dell'utente o delle chiamate simultanee (in base al codice o script) per evitare il consumo eccessivo di risorse. Per ulteriori informazioni sulla limitazione, vedere Evitare di limitarsi o bloccarsi [in SharePoint Online.](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- Se si verificano  prestazioni lente con un sito **o** una pagina SharePoint classica o moderna, utilizzare lo strumento [Diagnostica pagine](https://aka.ms/perftool) per analizzare le pagine.
  
- Se si verificano ancora prestazioni lente [generali,](https://go.microsoft.com/fwlink/?linkid=2024334) consultare le risorse nella parte inferiore di questo articolo: Introduzione all'ottimizzazione delle prestazioni per SharePoint Online
  