---
title: Come disabilitare gruppi esterni
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 4807dbfbabcea1f13785bd39bb48e4bbaa8d0f0f
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/15/2019
ms.locfileid: "28295994"
---
# <a name="how-to-disable-external-groups"></a>Come disabilitare gruppi esterni

Yammer messaggistica esterni si applica regole di trasporto Exchange (ETRs), un insieme di controlli proattivi per impedire che informazioni società condiviso. Per impedire agli utenti di creare gruppi esterni, è necessario configurare una regola di trasporto di Exchange (ETR) e quindi configurare Yammer per l'utilizzo della regola di trasporto di Exchange per bloccare la messaggistica esterno. 
  
Dopo aver creato una regola nell'interfaccia di amministrazione di Exchange Online, eseguire la procedura seguente per impostare ETR da applicare in Yammer:
  
- Accedere a Yammer come un amministratore verificato e nell' **interfaccia di amministrazione di Yammer**, andare alla C **obbligatoria e sicurezza \> le impostazioni di sicurezza.**
    
- In **Messaggistica esterno**, selezionare **applicare i Exchange Transport Rules Exchange Online (ETRs) in Yammer.**
    
- Scegliere **Save**. 
    
Per ulteriori informazioni, vedere [controllo esterno messaggistica in una rete Yammer con le regole di trasporto di Exchange](https://support.office.com/en-us/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)
  

