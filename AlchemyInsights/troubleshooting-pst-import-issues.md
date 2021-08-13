---
title: Risoluzione dei problemi di importazione PST
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1225"
ms.openlocfilehash: 549af832f9c58db1cdd8fbe80b8b5bd2aba9bd937f33116806a9391cbc9a5d4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972423"
---
# <a name="troubleshooting-pst-import-issues"></a>Risoluzione dei problemi di importazione PST

- Se stai eseguendo l'importazione nel client di Outlook stesso, vedi [Risolvere i problemi importando un file PST in Outlook](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).

- Se il servizio di importazione si è bloccato durante l'uso, considera che ogni file PST caricato nei percorsi di Archiviazione di Azure non deve essere più grande di 20 GB. I file PST più grandi di 20 GB possono influire sulle prestazioni del processo di importazione PST. Per altre informazioni sui processi di risoluzione dei problemi bloccati, vedi [Problemi che condizionano i processi di importazione dei file PST](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).

- Se vuoi verificare lo stato di uno specifico processo di importazione, usa [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).

- Per informazioni complete sul servizio di importazione, vedere [Panoramica sull'importazione di file PST dell'organizzazione](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).
