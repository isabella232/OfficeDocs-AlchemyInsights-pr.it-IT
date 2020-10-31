---
title: errore 0x8004de40 durante l'avvio di OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 10/30/2020
ms.locfileid: "48815993"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="504b5-102">errore 0x8004de40 durante l'avvio di OneDrive</span><span class="sxs-lookup"><span data-stu-id="504b5-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="504b5-103">Se viene visualizzato un messaggio di errore **0x8004de40** durante l'accesso a OneDrive, riavviare il computer quando si è connessi al dominio di lavoro o della scuola.</span><span class="sxs-lookup"><span data-stu-id="504b5-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="504b5-104">Se si riceve questo errore dopo il riavvio, provare a eseguire questa operazione quando si è connessi al dominio di lavoro o della scuola:</span><span class="sxs-lookup"><span data-stu-id="504b5-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="504b5-105">Fare clic sul pulsante Start e digitare **cmd** o **prompt dei comandi**  nella casella di ricerca, fare clic con il pulsante destro del mouse sull'app del prompt dei comandi e scegliere  **Esegui come amministratore** .</span><span class="sxs-lookup"><span data-stu-id="504b5-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator** .</span></span> <span data-ttu-id="504b5-106">Se viene richiesta una password di amministratore o per una conferma, digitare la password oppure fare clic su **Consenti** .</span><span class="sxs-lookup"><span data-stu-id="504b5-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow** .</span></span>  

2. <span data-ttu-id="504b5-107">Nella finestra del prompt dei comandi digitare **dsregcmd/Leave**  e attendere il completamento del comando.</span><span class="sxs-lookup"><span data-stu-id="504b5-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="504b5-108">Digitare **dsregcmd/join** e attendere il completamento del comando.</span><span class="sxs-lookup"><span data-stu-id="504b5-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="504b5-109">Riavviare il computer.</span><span class="sxs-lookup"><span data-stu-id="504b5-109">Reboot your computer.</span></span>
