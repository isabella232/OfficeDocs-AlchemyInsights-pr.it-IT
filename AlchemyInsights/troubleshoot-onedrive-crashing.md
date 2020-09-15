---
title: Risolvere i problemi di arresto anomalo di OneDrive
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
- "9003084"
- "5885"
ms.openlocfilehash: 1155d370911b28bbb1ba83a15eace66d1daea28f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665002"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="f7e0d-102">Risolvere i problemi di arresto anomalo di OneDrive</span><span class="sxs-lookup"><span data-stu-id="f7e0d-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="f7e0d-103">Se OneDrive si arresta spesso in modo anomalo, provare queste procedure per la risoluzione dei problemi:</span><span class="sxs-lookup"><span data-stu-id="f7e0d-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="f7e0d-104">**Assicurarsi che non siano impostate chiavi del Registro di sistema:**</span><span class="sxs-lookup"><span data-stu-id="f7e0d-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="f7e0d-105">Usando l'Editor del Registro di sistema, passare a HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="f7e0d-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="f7e0d-106">Se è presente la chiave DisableFileSyncNGSC con il valore impostato su 1, aprire la chiave e cambiare il valore in 0.</span><span class="sxs-lookup"><span data-stu-id="f7e0d-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="f7e0d-107">Avviare manualmente OneDrive facendo clic su Start</span><span class="sxs-lookup"><span data-stu-id="f7e0d-107">Manually launch OneDrive by going to Start</span></span> ![Premere il tasto WINDOWS](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="f7e0d-109">, digitare OneDrive nella casella di ricerca e quindi fare clic sull'app OneDrive desktop.</span><span class="sxs-lookup"><span data-stu-id="f7e0d-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="f7e0d-110">**Reimpostare OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="f7e0d-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="f7e0d-111">Note:</span><span class="sxs-lookup"><span data-stu-id="f7e0d-111">Notes:</span></span>

- <span data-ttu-id="f7e0d-112">La reimpostazione di OneDrive disconnette tutte le connessioni di sincronizzazione esistenti (incluso OneDrive personale, se configurato).</span><span class="sxs-lookup"><span data-stu-id="f7e0d-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="f7e0d-113">Quando si reimposta OneDrive nel computer, i file e i dati vengono preservati.</span><span class="sxs-lookup"><span data-stu-id="f7e0d-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="f7e0d-114">**Per reimpostare OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="f7e0d-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="f7e0d-115">Aprire una finestra di dialogo Esegui premendo il tasto WINDOWS e R.</span><span class="sxs-lookup"><span data-stu-id="f7e0d-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="f7e0d-116">Digitare %localappdata%\Microsoft\OneDrive\onedrive.exe /reset e scegliere OK.</span><span class="sxs-lookup"><span data-stu-id="f7e0d-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="f7e0d-117">Potrebbe comparire una finestra di comando per un istante.</span><span class="sxs-lookup"><span data-stu-id="f7e0d-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="f7e0d-118">Avviare manualmente OneDrive facendo clic su Start</span><span class="sxs-lookup"><span data-stu-id="f7e0d-118">Manually launch OneDrive by going to Start</span></span> ![Premere il tasto WINDOWS](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="f7e0d-120">, digitare OneDrive nella casella di ricerca e quindi fare clic sull'app OneDrive desktop.</span><span class="sxs-lookup"><span data-stu-id="f7e0d-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="f7e0d-121">Note:</span><span class="sxs-lookup"><span data-stu-id="f7e0d-121">Notes:</span></span>

- <span data-ttu-id="f7e0d-122">Se prima del ripristino era stata impostata la sincronizzazione solo di alcune cartelle, si dovrà applicare di nuovo questa impostazione al termine della sincronizzazione.</span><span class="sxs-lookup"><span data-stu-id="f7e0d-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="f7e0d-123">Per altre informazioni, vedere [Scegliere le cartelle di OneDrive da sincronizzare con il computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) .</span><span class="sxs-lookup"><span data-stu-id="f7e0d-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="f7e0d-124">È necessario completare la procedura per OneDrive personale e OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="f7e0d-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>