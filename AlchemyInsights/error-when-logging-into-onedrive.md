---
title: 0x8004de40 errore durante l'avvio di OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: e329d7fe881a0fc9514584e06aa2d6e8ebab5b11
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813656"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="5e1e9-102">0x8004de40 errore durante l'avvio di OneDrive</span><span class="sxs-lookup"><span data-stu-id="5e1e9-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="5e1e9-103">Se viene visualizzato un messaggio di **0x8004de40** durante l'accesso a OneDrive, riavviare il computer mentre si è connessi al dominio dell'istituto di istruzione o dell'istituto di istruzione.</span><span class="sxs-lookup"><span data-stu-id="5e1e9-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="5e1e9-104">Se viene visualizzato questo errore dopo il riavvio, provare a eseguire questa operazione mentre si è connessi al dominio dell'istituto di istruzione o dell'istituto di istruzione:</span><span class="sxs-lookup"><span data-stu-id="5e1e9-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="5e1e9-105">Fare clic sul pulsante Start e digitare **cmd** o **prompt** dei comandi nella casella di ricerca, fare clic con il pulsante destro del mouse sull'app del prompt dei comandi e scegliere **Esegui come amministratore.**</span><span class="sxs-lookup"><span data-stu-id="5e1e9-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator**.</span></span> <span data-ttu-id="5e1e9-106">Se viene richiesta una password di amministratore o una conferma, digitare la password o fare clic su **Consenti**.</span><span class="sxs-lookup"><span data-stu-id="5e1e9-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow**.</span></span>  

2. <span data-ttu-id="5e1e9-107">Nella finestra del prompt dei comandi digitare **dsregcmd /leave**  e attendere il completamento del comando.</span><span class="sxs-lookup"><span data-stu-id="5e1e9-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="5e1e9-108">Digitare **quindi dsregcmd /join e** attendere il completamento del comando.</span><span class="sxs-lookup"><span data-stu-id="5e1e9-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="5e1e9-109">Riavviare il computer.</span><span class="sxs-lookup"><span data-stu-id="5e1e9-109">Reboot your computer.</span></span>
