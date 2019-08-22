---
title: FIX 0x8004de40 Error in OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: d436184bdc0e283db217ea734fb2c8e05f85b4e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525063"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="f9aef-102">FIX 0x8004de40 Error in OneDrive</span><span class="sxs-lookup"><span data-stu-id="f9aef-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="f9aef-103">Se viene visualizzato un errore di 0x8004de40 con OneDrive:</span><span class="sxs-lookup"><span data-stu-id="f9aef-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="f9aef-104">Riavviare il computer coinvolto quando si è connessi al dominio di directory di Acitve.</span><span class="sxs-lookup"><span data-stu-id="f9aef-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="f9aef-105">Se un riavvio non risolve il problema, disconnettersi e riaggiungere il dispositivo da Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f9aef-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="f9aef-106">**Nota**: durante l'esecuzione di questa procedura, è necessario essere presenti nella rete aziendale.</span><span class="sxs-lookup"><span data-stu-id="f9aef-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="f9aef-107">Non eseguire questi passaggi se non si è in grado di connettersi all'infrastruttura aziendale, ad esempio durante il viaggio.</span><span class="sxs-lookup"><span data-stu-id="f9aef-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="f9aef-108">Aprire un prompt dei comandi con privilegi elevati.</span><span class="sxs-lookup"><span data-stu-id="f9aef-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="f9aef-109">Per aprire un prompt dei comandi con privilegi elevati, fare clic su **Start**, fare clic con il pulsante destro del mouse su **prompt dei comandi**e quindi scegliere **Esegui come amministratore**.</span><span class="sxs-lookup"><span data-stu-id="f9aef-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="f9aef-110">Digitare *dsregcmd/Leave* e premere **invio**.</span><span class="sxs-lookup"><span data-stu-id="f9aef-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="f9aef-111">Al termine, digitare *dsregcmd/join* e premere **invio**.</span><span class="sxs-lookup"><span data-stu-id="f9aef-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="f9aef-112">Al termine, chiudere la finestra del prompt dei comandi.</span><span class="sxs-lookup"><span data-stu-id="f9aef-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="f9aef-113">Riavviare il computer ed eseguire l'accesso a OneDrive.</span><span class="sxs-lookup"><span data-stu-id="f9aef-113">Reboot the computer, and log into OneDrive.</span></span>