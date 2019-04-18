---
title: Risoluzione dei problemi relativi all'errore 404, file non trovato
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 1b15444c-367b-4523-8e08-1c77bbea7524
ms.openlocfilehash: 467feb3cb436a2e0135162657876e5c45d8d56bd
ms.sourcegitcommit: 228c986911ecf73217116a5d1fdcd2e89362774e
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/09/2019
ms.locfileid: "31747243"
---
# <a name="troubleshoot-error-404-file-not-found"></a><span data-ttu-id="a0a38-102">Risoluzione dei problemi relativi all'errore 404, file non trovato</span><span class="sxs-lookup"><span data-stu-id="a0a38-102">Troubleshoot Error 404, File not found</span></span>

<span data-ttu-id="a0a38-103">Viene ricevuto un errore 404 quando gli utenti tentano di accedere a un sito o a un file in SharePoint o OneDrive.</span><span class="sxs-lookup"><span data-stu-id="a0a38-103">An Error 404 is received when users are attempting to access a site or file in SharePoint or OneDrive.</span></span> <span data-ttu-id="a0a38-104">Questo è spesso causato da un sito o un file o un gruppo che viene rinominato, spostato o eliminato.</span><span class="sxs-lookup"><span data-stu-id="a0a38-104">This is often caused by a site or file or group getting renamed, moved or deleted.</span></span> <span data-ttu-id="a0a38-105">Ad esempio, gli utenti sperimenteranno un errore 404 che tenta di accedere alla raccolta siti radice ed è stata eliminata.</span><span class="sxs-lookup"><span data-stu-id="a0a38-105">For example: Users will experience a 404 Error attempting to access the Root Site Collection and it has been deleted.</span></span>

<span data-ttu-id="a0a38-106">Per risolvere l'errore 404 per un sito che è stato rinominato, spostato o eliminato:</span><span class="sxs-lookup"><span data-stu-id="a0a38-106">To resolve Error 404 for a Site that has been renamed, moved or deleted:</span></span>

<span data-ttu-id="a0a38-107">Per i siti classici presenti nell'interfaccia di amministrazione classica, vedere [ripristinare una raccolta siti eliminata](https://docs.microsoft.com/en-us/sharepoint/restore-deleted-site-collection).</span><span class="sxs-lookup"><span data-stu-id="a0a38-107">For classic sites that exist in the Classic Admin Center, see [Restore a deleted site collection](https://docs.microsoft.com/en-us/sharepoint/restore-deleted-site-collection).</span></span>


<span data-ttu-id="a0a38-108">Per i siti moderni (comunicazioni, gruppi o altri siti) presenti nella nuova interfaccia di amministrazione di SharePoint, vedere [View and Restore Deleted sites in the New SharePoint Admin Center](https://docs.microsoft.com/en-us/sharepoint/restore-deleted-site-collection).</span><span class="sxs-lookup"><span data-stu-id="a0a38-108">For modern sites (communication, group-connected, or other sites) that exist in the new SharePoint admin center, see [View and restore deleted sites in the new SharePoint admin center](https://docs.microsoft.com/en-us/sharepoint/restore-deleted-site-collection).</span></span>

<span data-ttu-id="a0a38-109">Per risolvere l'errore 404 per un file o un altro elemento che è stato rinominato, spostato o eliminato:</span><span class="sxs-lookup"><span data-stu-id="a0a38-109">To resolve Error 404 for a File (or other item) that has been renamed, moved or deleted:</span></span>

<span data-ttu-id="a0a38-110">Passare al sito di SharePoint o OneDrive e visualizzare il cestino dal contenuto del sito.</span><span class="sxs-lookup"><span data-stu-id="a0a38-110">Go to the SharePoint or OneDrive site and view the Recycle Bin from the Site contents.</span></span> <span data-ttu-id="a0a38-111">Vedere, [ripristinare gli elementi nel cestino di un sito di SharePoint](https://support.office.com/en-us/article/Restore-items-in-the-Recycle-Bin-of-a-SharePoint-site-6df466b6-55f2-4898-8d6e-c0dff851a0be#ID0EAADAAA=Online).</span><span class="sxs-lookup"><span data-stu-id="a0a38-111">See, [Restore items in the Recycle Bin of a SharePoint site](https://support.office.com/en-us/article/Restore-items-in-the-Recycle-Bin-of-a-SharePoint-site-6df466b6-55f2-4898-8d6e-c0dff851a0be#ID0EAADAAA=Online).</span></span>

<span data-ttu-id="a0a38-112">Se non si è ancora in grado di individuare l'elemento, è possibile eseguire una ricerca nel registro di controllo se è abilitata la registrazione vedere, [cercare nel log di controllo nel centro conformità di Office 365 Security &](https://docs.microsoft.com/en-us/office365/securitycompliance/search-the-audit-log-in-security-and-compliance?redirectSourcePath=%252fclient%252fsearch-the-audit-log-in-the-office-365-security-compliance-center-0d4d0f35-390b-4518-800e-0c7ec95e946c).</span><span class="sxs-lookup"><span data-stu-id="a0a38-112">If you are still unable to find the item you can search the audit log if logging is enabled see, [Search the audit log in the Office 365 Security & Compliance Center](https://docs.microsoft.com/en-us/office365/securitycompliance/search-the-audit-log-in-security-and-compliance?redirectSourcePath=%252fclient%252fsearch-the-audit-log-in-the-office-365-security-compliance-center-0d4d0f35-390b-4518-800e-0c7ec95e946c).</span></span>