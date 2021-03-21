---
title: Diagnostica dei problemi di accesso a porte diverse
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9035"
- "9005220"
ms.openlocfilehash: 3673067cad7ac55f3820422dc2ec09942c393149
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897876"
---
# <a name="diagnostics-for-different-ports-access-issues"></a><span data-ttu-id="441dd-102">Diagnostica dei problemi di accesso a porte diverse</span><span class="sxs-lookup"><span data-stu-id="441dd-102">Diagnostics for different ports access issues</span></span>

<span data-ttu-id="441dd-103">Per risolvere i problemi di accesso a porte diverse, seguire questa procedura:</span><span class="sxs-lookup"><span data-stu-id="441dd-103">To resolve the different port access issues, perform the following steps:</span></span>

1. <span data-ttu-id="441dd-104">Arrestare/deallocare la macchina virtuale (VM) dal portale, riavviare la VM e ripetere il test.</span><span class="sxs-lookup"><span data-stu-id="441dd-104">Stop/deallocate the virtual machine (VM) from the portal, restart the VM, and test again.</span></span> 
2. <span data-ttu-id="441dd-105">Controllare le impostazioni di rete della VM per determinare se i gruppi di sicurezza di rete bloccano il traffico.</span><span class="sxs-lookup"><span data-stu-id="441dd-105">Check your VM's network settings to determine if you have Network Security Groups (NSGs) blocking traffic.</span></span> <span data-ttu-id="441dd-106">È anche possibile usare lo [strumento di verifica del flusso IP di Network Watcher](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) per verificare se ci sono messaggi di mancato recapito che bloccano il traffico, route definite dall'utente che reindirizzano il traffico verso la connessione locale ('Route predefinita' 0.0.0.0/0) o un appliance di rete.</span><span class="sxs-lookup"><span data-stu-id="441dd-106">You can also use [Network Watcher's IP flow verify tool](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) to check for NSGs blocking traffic, User-Defined Routes (UDRs) rerouting your traffic back to on-premises ('Default Route' 0.0.0.0/0), or to a network appliance.</span></span>
<span data-ttu-id="441dd-107">Se si verificano ancora problemi dopo aver provato a eseguire i passaggi precedenti, specificare il nome della VM e la porta TCP su cui si sta provando a inviare messaggi per procedere con un'ulteriore diagnosi.</span><span class="sxs-lookup"><span data-stu-id="441dd-107">If you still experience issues after trying the steps above, please provide the VM name and the TCP port you are attempting to send mail on for further diagnosis.</span></span>

<span data-ttu-id="441dd-108">**Documenti consigliati**</span><span class="sxs-lookup"><span data-stu-id="441dd-108">**Recommended Documents**</span></span>

[<span data-ttu-id="441dd-109">Limitazioni e consigli per l'invio di posta elettronica in uscita sulla porta 25</span><span class="sxs-lookup"><span data-stu-id="441dd-109">Limitations and recommendations for sending outbound email over port 25</span></span>](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)