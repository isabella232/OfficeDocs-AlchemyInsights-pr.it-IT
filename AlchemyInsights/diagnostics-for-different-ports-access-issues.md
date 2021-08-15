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
ms.openlocfilehash: 07c108d5292965d20340da039b67744d93c0a4fc61edb8115796671f2f7f1552
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030906"
---
# <a name="diagnostics-for-different-ports-access-issues"></a>Diagnostica dei problemi di accesso a porte diverse

Per risolvere i problemi di accesso a porte diverse, seguire questa procedura:

1. Arrestare/deallocare la macchina virtuale (VM) dal portale, riavviare la VM e ripetere il test. 
2. Controllare le impostazioni di rete della VM per determinare se i gruppi di sicurezza di rete bloccano il traffico. È anche possibile usare lo [strumento di verifica del flusso IP di Network Watcher](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) per verificare se ci sono messaggi di mancato recapito che bloccano il traffico, route definite dall'utente che reindirizzano il traffico verso la connessione locale ('Route predefinita' 0.0.0.0/0) o un appliance di rete.
Se si verificano ancora problemi dopo aver provato a eseguire i passaggi precedenti, specificare il nome della VM e la porta TCP su cui si sta provando a inviare messaggi per procedere con un'ulteriore diagnosi.

**Documenti consigliati**

[Limitazioni e consigli per l'invio di posta elettronica in uscita sulla porta 25](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)