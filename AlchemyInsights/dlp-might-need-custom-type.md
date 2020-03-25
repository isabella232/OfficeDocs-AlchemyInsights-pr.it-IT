---
title: DLP potrebbe essere necessario un tipo personalizzato
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 890bba57bc36c034c507e6124cd6593ef4d92af8
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932662"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP potrebbe essere necessario un tipo personalizzato

**Importante**: molti clienti di SharePoint Online e OneDrive eseguono applicazioni aziendali critiche rispetto al servizio in esecuzione in background. Tali applicazioni includono soluzioni per la migrazione del contenuto, di Prevenzione della perdita dei dati e per il backup. In questi tempi straordinari, stiamo adottando misure per garantire che i servizi di SharePoint Online e OneDrive rimangano altamente disponibili e affidabili per gli utenti che dipendono ancor più dal servizio negli scenari di lavoro remoto.

A sostegno di questo obiettivo, abbiamo implementato limitazioni più rigide sulle app in background (migrazione, prevenzione della perdita dei dati e soluzioni di backup) durante il giorni nei giorni feriali. In questo periodo sarà possibile notare una riduzione della velocità effettiva in queste app. Tuttavia, nelle ore serali e durante il fine settimana nell'area il servizio sarà predisposto per elaborare una quantità notevolmente superiore di richieste delle app in background.

**DLP potrebbe richiedere un tipo di informazioni personalizzato**

Con un criterio di prevenzione della perdita di dati (DLP), è possibile identificare e proteggere i dati sensibili nell'organizzazione. In alcuni scenari potrebbe essere necessario creare un tipo di informazioni riservate **personalizzato** per proteggere i dati dell'organizzazione.

Ad esempio, è possibile che l'organizzazione debba identificare e proteggere gli ID dei dipendenti o altri dati in un formato specifico per l'org. In caso affermativo, vedere gli articoli seguenti per ulteriori informazioni.
  
 **Personalizzare una tipologia integrata di informazioni sensibili**
  
Se un tipo di informazioni riservate incorporato soddisfa le proprie esigenze con solo alcuni ritocchi, è possibile [personalizzare un tipo di informazioni riservate incorporato](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type). Ad esempio, è possibile aggiungere o rimuovere parole chiave oppure aggiungere o rimuovere elementi di prova di supporto quali una data o un indirizzo.
  
 **Creare una tipologia personalizzata di informazioni riservate**
  
Tuttavia, se è necessario identificare e proteggere complessivamente un tipo diverso di informazioni riservate, è possibile [creare un tipo di informazioni riservate personalizzato](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) nell'interfaccia utente del centro sicurezza & conformità.
  
**Creare un tipo di informazioni sensibili personalizzato in PowerShell per Centro sicurezza e conformità**

Infine, se l'interfaccia utente non fornisce tutte le opzioni necessarie, è possibile [creare un tipo di informazioni riservate personalizzato nel centro sicurezza & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell). Se si inizia con un file XML, è possibile utilizzare tutte le opzioni disponibili.
