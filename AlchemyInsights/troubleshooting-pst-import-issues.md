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
# <a name="troubleshooting-pst-import-issues"></a><span data-ttu-id="a3ca7-102">Risoluzione dei problemi di importazione PST</span><span class="sxs-lookup"><span data-stu-id="a3ca7-102">Troubleshooting PST import issues</span></span>

- <span data-ttu-id="a3ca7-103">Se si sta eseguendo l'importazione nel client Outlook, vedere [Risolvere i problemi di importazione di un file PST di Outlook](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span><span class="sxs-lookup"><span data-stu-id="a3ca7-103">If you are importing within the Outlook client itself, please see [Fix problems importing an Outlook .pst file](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span></span>

- <span data-ttu-id="a3ca7-104">Se si usa il servizio di importazione e si è bloccato, tenere presente che le dimensioni di ogni file PST caricato nella posizione di archiviazione di Azure non devono essere superiori a 20 GB.</span><span class="sxs-lookup"><span data-stu-id="a3ca7-104">If you are using Import Service and it is stuck, please note that each PST file that you upload to the Azure Storage location should be no larger than 20 GB.</span></span> <span data-ttu-id="a3ca7-105">I file PST più grandi di 20 GB possono influire sulle prestazioni del processo di importazione PST.</span><span class="sxs-lookup"><span data-stu-id="a3ca7-105">PST files larger than 20 GB may impact the performance of the PST import process.</span></span>

- <span data-ttu-id="a3ca7-106">Se si vuole verificare lo stato di uno specifico processo di importazione, è possibile usare [Get-MailboxImportRequest-BatchName](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span><span class="sxs-lookup"><span data-stu-id="a3ca7-106">If you want to verify the status of a specific Import job, you can use [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span></span>

- <span data-ttu-id="a3ca7-107">Per informazioni complete sul servizio di importazione, vedere [Panoramica dell'importazione di file PST dell'organizzazione](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="a3ca7-107">For full details on the import service, please see [Overview of importing your organization's PST files](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span></span>
