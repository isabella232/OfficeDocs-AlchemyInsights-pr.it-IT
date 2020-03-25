---
title: Limitazione di SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: 9af4f09d50992c04a1f3d5a164093049a3ec3517
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931446"
---
# <a name="sharepoint-online-throttling"></a>Limitazione di SharePoint Online

**Importante**: molti clienti di SharePoint Online e OneDrive eseguono applicazioni aziendali critiche rispetto al servizio in esecuzione in background. Tali applicazioni includono soluzioni per la migrazione del contenuto, di Prevenzione della perdita dei dati e per il backup. In questi tempi straordinari, stiamo adottando misure per garantire che i servizi di SharePoint Online e OneDrive rimangano altamente disponibili e affidabili per gli utenti che dipendono ancor più dal servizio negli scenari di lavoro remoto.

A sostegno di questo obiettivo, abbiamo implementato limitazioni più rigide sulle app in background (migrazione, prevenzione della perdita dei dati e soluzioni di backup) durante il giorni nei giorni feriali. In questo periodo sarà possibile notare una riduzione della velocità effettiva in queste app. Tuttavia, nelle ore serali e durante il fine settimana nell'area il servizio sarà predisposto per elaborare una quantità notevolmente superiore di richieste delle app in background.

**Limitazione di SharePoint Online**

SharePoint Online utilizza la limitazione per mantenere le prestazioni ottimali e l'affidabilità del servizio SharePoint Online. La limitazione limita il numero di azioni utente o di chiamate simultanee (tramite script o codice) per impedire un utilizzo eccessivo delle risorse. Per ulteriori informazioni, visitare i collegamenti riportati di seguito.

- [Evitare la limitazione o il blocco in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [Migrazione dei dati e limitazione di SPO](https://blogs.technet.microsoft.com/sposupport/2017/08/12/data-migration-and-spo-service-throttling/)

- [Velocità di migrazione in SharePoint Online e OneDrive](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

 - [Gestire la limitazione di SharePoint Online utilizzando la retromarcia esponenziale](https://docs.microsoft.com/sharepoint/dev/solution-guidance/handle-sharepoint-online-throttling-by-using-exponential-back-off)

- [Pianificazione della capacità e test di carico di SharePoint Online](https://docs.microsoft.com/office365/enterprise/capacity-planning-and-load-testing-sharepoint-online)

