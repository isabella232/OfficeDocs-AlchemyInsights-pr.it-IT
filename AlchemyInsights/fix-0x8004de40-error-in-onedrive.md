---
title: FIX 0x8004de40 Error in OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 5da4271f242597b195ef61d553fd4a2ffb313025
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716032"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="47f45-102">FIX 0x8004de40 Error in OneDrive</span><span class="sxs-lookup"><span data-stu-id="47f45-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="47f45-103">Se viene visualizzato un errore di 0x8004de40 con OneDrive:</span><span class="sxs-lookup"><span data-stu-id="47f45-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="47f45-104">Riavviare il computer coinvolto quando si è connessi al dominio di directory di Acitve.</span><span class="sxs-lookup"><span data-stu-id="47f45-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="47f45-105">Se un riavvio non risolve il problema, disconnettersi e riaggiungere il dispositivo da Azure AD.</span><span class="sxs-lookup"><span data-stu-id="47f45-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="47f45-106">**Nota**: durante l'esecuzione di questa procedura, è necessario essere presenti nella rete aziendale.</span><span class="sxs-lookup"><span data-stu-id="47f45-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="47f45-107">Non eseguire questi passaggi se non si è in grado di connettersi all'infrastruttura aziendale, ad esempio durante il viaggio.</span><span class="sxs-lookup"><span data-stu-id="47f45-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="47f45-108">Aprire un prompt dei comandi con privilegi elevati.</span><span class="sxs-lookup"><span data-stu-id="47f45-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="47f45-109">Per aprire un prompt dei comandi con privilegi elevati, fare clic su **Start**, fare clic con il pulsante destro del mouse su **prompt dei comandi**e quindi scegliere **Esegui come amministratore**.</span><span class="sxs-lookup"><span data-stu-id="47f45-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="47f45-110">Digitare *dsregcmd/Leave* e premere **invio**.</span><span class="sxs-lookup"><span data-stu-id="47f45-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="47f45-111">Al termine, digitare *dsregcmd/join* e premere **invio**.</span><span class="sxs-lookup"><span data-stu-id="47f45-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="47f45-112">Al termine, chiudere la finestra del prompt dei comandi.</span><span class="sxs-lookup"><span data-stu-id="47f45-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="47f45-113">Riavviare il computer ed eseguire l'accesso a OneDrive.</span><span class="sxs-lookup"><span data-stu-id="47f45-113">Reboot the computer, and log into OneDrive.</span></span>