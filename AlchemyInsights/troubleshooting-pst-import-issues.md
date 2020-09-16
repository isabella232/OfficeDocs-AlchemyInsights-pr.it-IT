---
title: Risoluzione dei problemi di importazione PST
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1225"
ms.openlocfilehash: 5fdb713f321e5c9f67a6078739c31a90571b913d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47757744"
---
# <a name="troubleshooting-pst-import-issues"></a>Risoluzione dei problemi di importazione PST

- Se si sta eseguendo l'importazione nel client Outlook, vedere [Risolvere i problemi di importazione di un file PST di Outlook](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).

- Se si usa il servizio di importazione e si è bloccato, tenere presente che le dimensioni di ogni file PST caricato nella posizione di archiviazione di Azure non devono essere superiori a 20 GB. I file PST più grandi di 20 GB possono influire sulle prestazioni del processo di importazione PST.

- Se si vuole verificare lo stato di uno specifico processo di importazione, è possibile usare [Get-MailboxImportRequest-BatchName](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).

- Per informazioni complete sul servizio di importazione, vedere [Panoramica dell'importazione di file PST dell'organizzazione](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).
