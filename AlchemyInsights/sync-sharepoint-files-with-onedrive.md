---
title: Risolvere i problemi con "Apri con Esplora risorse" in SharePoint Online
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 8/7/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 5ad2f1f2-9650-4eb0-b4fa-2f52a09f535a
ms.openlocfilehash: afee367e250357b20b77f0ea5dfe66d68967eb2a
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270712"
---
# <a name="troubleshoot-open-with-explorer-issues-in-sharepoint-online"></a><span data-ttu-id="1fc1c-102">Risolvere i problemi con "Apri con Esplora risorse" in SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="1fc1c-102">Troubleshoot “Open with Explorer” issues in SharePoint Online</span></span>

<span data-ttu-id="1fc1c-103">Il comando Apri con Esplora risorse apre un'istanza locale di Esplora risorse che mostra la struttura delle cartelle nel server che ospita il sito di SharePoint.</span><span class="sxs-lookup"><span data-stu-id="1fc1c-103">The Open with Explorer command opens a local instance of Windows Explorer that displays the folder structure on the server that hosts the SharePoint site.</span></span> <span data-ttu-id="1fc1c-104">Detto questo, è consigliabile [sincronizzare i file di SharePoint con il nuovo client di sincronizzazione di OneDrive](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a>, che fornisce [File su richiesta](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) perché permette l'accesso locale ai file e offre prestazioni migliori.</span><span class="sxs-lookup"><span data-stu-id="1fc1c-104">This being said, we recommend [syncing SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) because it provides local access to your files and offers the best performance.</span></span>


<span data-ttu-id="1fc1c-105">Se si è scelto di usare la visualizzazione Esplora risorse invece di usare il nuovo client di sincronizzazione di OneDrive, assicurarsi di seguire i passaggi e le procedure consigliate descritti negli articoli seguenti:</span><span class="sxs-lookup"><span data-stu-id="1fc1c-105">If you chose to use Explorer view instead of using the new OneDrive sync client, make sure you follow the steps and best practices in the following articles:</span></span>

- [<span data-ttu-id="1fc1c-106">Come usare il comando "Apri con Esplora risorse" per risolvere i problemi in SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="1fc1c-106">How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online</span></span>](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4)

- [<span data-ttu-id="1fc1c-107">Copiare o spostare file delle raccolte tramite Apri con Esplora risorse</span><span class="sxs-lookup"><span data-stu-id="1fc1c-107">Copy or move library files by using Open with Explorer</span></span>](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2)

> [!Note]  
> <span data-ttu-id="1fc1c-108">Il pulsante **Apri con Esplora risorse** non è presente nella nuova esperienza di libreria.</span><span class="sxs-lookup"><span data-stu-id="1fc1c-108">The **Open with Explorer** button doesn't appear in the new library experience.</span></span> <span data-ttu-id="1fc1c-109">Fare clic sull'elenco a discesa **Visualizzazione** in alto a destra (il nome di questo elenco cambia a seconda della visualizzazione corrente) e poi selezionare **Visualizza in Esplora risorse**.</span><span class="sxs-lookup"><span data-stu-id="1fc1c-109">Select the **View** drop-down in the upper right (the name of the drop-down changes depending on your current view), and then select **View in File Explorer**.</span></span>
>
 ><span data-ttu-id="1fc1c-110">Apri con Esplora risorse di SharePoint usa i controlli ActiveX, quindi è supportato solo in Internet Explorer 10 o 11.</span><span class="sxs-lookup"><span data-stu-id="1fc1c-110">SharePoint Open with Explorer uses ActiveX controls, so it's only supported in Internet Explorer 10 or 11.</span></span> <span data-ttu-id="1fc1c-111">Apri con Esplora risorse non funziona in Windows con Microsoft Edge, Google Chrome, Mozilla Firefox, né sulla piattaforma Mac.</span><span class="sxs-lookup"><span data-stu-id="1fc1c-111">Open with Explorer doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="1fc1c-112">Per questo motivo, l'opzione di visualizzazione Esplora risorse potrebbe essere inattiva.</span><span class="sxs-lookup"><span data-stu-id="1fc1c-112">Due to this reason, the Explorer View option may be grayed out.</span></span>
>
> - <span data-ttu-id="1fc1c-113">[Motivi per cui i pulsanti della barra multifunzione di SharePoint non sono disponibili o sono inattivi](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span><span class="sxs-lookup"><span data-stu-id="1fc1c-113">[Why SharePoint ribbon buttons are unavailable or grayed out](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span></span>
  

