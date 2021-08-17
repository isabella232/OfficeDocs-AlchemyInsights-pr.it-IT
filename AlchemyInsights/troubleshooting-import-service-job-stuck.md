---
title: Risoluzione dei problemi relativi al blocco dei processi di importazione
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/27/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7907"
- "9003046"
ms.openlocfilehash: bf07102d01d85eaed8ea95b571a0eabea7c4b7448839294f37e5e30134e04282
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105104"
---
# <a name="troubleshooting-import-service-job-stuck"></a>Risoluzione dei problemi relativi al blocco dei processi di importazione

Se stai riscontrando problemi con il blocco o la mancata esecuzione dei servizi, esamina e prova quanto segue:

- Controlla la dimensione del file PST. La dimensione massima raccomandata dei file PST per l'importazione è 20 GB.

- Se sospetti di avere saltato degli elementi danneggiati, esegui Scanpst.exe per diagnosticare e risolvere i problemi dei file PST.

- Se riscontri un errore "MapiExceptionShutoffQuotaExceeded" durante l'importazione, assicurati che la capacità della cassetta postale di destinazione sia sufficiente per importare i tuoi file PST.

Per altre informazioni sulla risoluzione dei problemi dei processi di importazione dei file PST, vedi [Risoluzione dei problemi dei processi di importazione dei file PST](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).

Per informazioni sulla risoluzione dei problemi di importazione dei file PST in Outlook, vedi [Risolvere i problemi di importazione dei file PST in Outlook (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us).