---
title: Correggere 0x8004de40 errore in OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649752"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="1e084-102">Correggere 0x8004de40 errore in OneDrive</span><span class="sxs-lookup"><span data-stu-id="1e084-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="1e084-103">Se stai eseguendo Windows 7 e ricevi questo errore, aggiorna per abilitare [TLS 1.1 e TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)come protocolli sicuri predefiniti in WinHTTP in Windows .</span><span class="sxs-lookup"><span data-stu-id="1e084-103">If you're running Windows 7 and receive this error, [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

<span data-ttu-id="1e084-104">Se si esegue Windows 10 e si riceve un 0x8004de40 con OneDrive:</span><span class="sxs-lookup"><span data-stu-id="1e084-104">If you're running Windows 10, and you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="1e084-105">Riavviare il computer interessato mentre si è connessi al dominio Acitve Directory.</span><span class="sxs-lookup"><span data-stu-id="1e084-105">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="1e084-106">Se un riavvio non risolve il problema, scollegati e ricongiungerti al dispositivo da Azure AD.</span><span class="sxs-lookup"><span data-stu-id="1e084-106">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="1e084-107">**Nota:** è consigliabile essere nella rete aziendale durante l'esecuzione di questi passaggi.</span><span class="sxs-lookup"><span data-stu-id="1e084-107">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="1e084-108">Non eseguire questi passaggi quando non sei connesso all'infrastruttura aziendale (ad esempio, durante i viaggi).</span><span class="sxs-lookup"><span data-stu-id="1e084-108">Don't perform these steps when you aren't connected to your corporate infrastructure (for example, while traveling).</span></span> 

1. <span data-ttu-id="1e084-109">Aprire un prompt dei comandi con privilegi elevati selezionando **Start**, fare clic con il pulsante destro del mouse su Prompt dei **comandi** e quindi scegliere Esegui **come amministratore**.</span><span class="sxs-lookup"><span data-stu-id="1e084-109">Open an elevated command prompt by selecting **Start**, right-click **Command Prompt**, and then select **Run as administrator**.</span></span>

1. <span data-ttu-id="1e084-110">Digitare *dsregcmd /leave* e premere **INVIO.**</span><span class="sxs-lookup"><span data-stu-id="1e084-110">Type *dsregcmd /leave* and press **Enter**.</span></span>

1. <span data-ttu-id="1e084-111">Al termine, digitare *dsregcmd /join* e premere **INVIO.**</span><span class="sxs-lookup"><span data-stu-id="1e084-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>

1. <span data-ttu-id="1e084-112">Al termine, chiudere il prompt dei comandi.</span><span class="sxs-lookup"><span data-stu-id="1e084-112">When complete, close the command prompt.</span></span>

1. <span data-ttu-id="1e084-113">Riavviare il computer ed eseguire l'accesso a OneDrive.</span><span class="sxs-lookup"><span data-stu-id="1e084-113">Reboot the computer, and log into OneDrive.</span></span>