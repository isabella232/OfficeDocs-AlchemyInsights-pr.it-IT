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
# <a name="diagnostics-for-different-ports-access-issues"></a>Diagnostica dei problemi di accesso a porte diverse

Per risolvere i problemi di accesso a porte diverse, seguire questa procedura:

1. Arrestare/deallocare la macchina virtuale (VM) dal portale, riavviare la VM e ripetere il test. 
2. Controllare le impostazioni di rete della VM per determinare se i gruppi di sicurezza di rete bloccano il traffico. È anche possibile usare lo [strumento di verifica del flusso IP di Network Watcher](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) per verificare se ci sono messaggi di mancato recapito che bloccano il traffico, route definite dall'utente che reindirizzano il traffico verso la connessione locale ('Route predefinita' 0.0.0.0/0) o un appliance di rete.
Se si verificano ancora problemi dopo aver provato a eseguire i passaggi precedenti, specificare il nome della VM e la porta TCP su cui si sta provando a inviare messaggi per procedere con un'ulteriore diagnosi.

**Documenti consigliati**

[Limitazioni e consigli per l'invio di posta elettronica in uscita sulla porta 25](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)