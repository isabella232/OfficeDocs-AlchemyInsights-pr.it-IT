---
title: Suggerimenti per i criteri DLP non funzionanti
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 51b4472fa721443192eb542cac45965df67634df
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932590"
---
# <a name="dlp-policy-tip-issues"></a>Problemi relativi ai suggerimenti per i criteri DLP

**Importante**: molti clienti di SharePoint Online e OneDrive eseguono applicazioni aziendali critiche rispetto al servizio in esecuzione in background. Tali applicazioni includono soluzioni per la migrazione del contenuto, di Prevenzione della perdita dei dati e per il backup. In questi tempi straordinari, stiamo adottando misure per garantire che i servizi di SharePoint Online e OneDrive rimangano altamente disponibili e affidabili per gli utenti che dipendono ancor più dal servizio negli scenari di lavoro remoto.

A sostegno di questo obiettivo, abbiamo implementato limitazioni più rigide sulle app in background (migrazione, prevenzione della perdita dei dati e soluzioni di backup) durante il giorni nei giorni feriali. In questo periodo sarà possibile notare una riduzione della velocità effettiva in queste app. Tuttavia, nelle ore serali e durante il fine settimana nell'area il servizio sarà predisposto per elaborare una quantità notevolmente superiore di richieste delle app in background.

**Suggerimenti per i criteri DLP**

Quando si utilizzano i **criteri DLP**, gli utenti possono ricevere la notifica di una violazione dei criteri con suggerimenti per i **criteri**. Gli amministratori possono configurare Suggerimenti per i criteri da visualizzare durante il testing del criterio DLP o quando il criterio è in modalità di applicazione completa.
  
Per configurare i suggerimenti per i criteri per i criteri DLP nel centro sicurezza e conformità in modalità di applicazione completa, eseguire le operazioni seguenti:
  
- Verificare che i suggerimenti per i criteri siano stati **abilitati** nella regola DLP utilizzando i passaggi riportati di [seguito](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).

- Verificare che il **contenuto corrisponda** a ciò che è **necessario** per attivare la regola descritta in [questo articolo.](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)

- I suggerimenti per i criteri vengono visualizzati sia in OWA che in Outlook. Tuttavia, quando si utilizza **Outlook 2013 o versione successiva**, i suggerimenti per i criteri vengono visualizzati solo in determinate condizioni. Queste condizioni sono elencate di seguito: [condizioni supportate per Outlook 2013 o versioni successive per la visualizzazione dei suggerimenti per i criteri](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)

Per ulteriori informazioni sui suggerimenti per i criteri DLP, vedere: [Mostra suggerimenti per i criteri per](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips) il criterio DLP
  