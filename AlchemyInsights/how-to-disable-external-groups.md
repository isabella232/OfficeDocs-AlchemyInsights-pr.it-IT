---
title: Come disabilitare i gruppi esterni
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 4683a71438ec31f9e9211404a9c66c4e45e0e1df
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36540905"
---
# <a name="how-to-disable-external-groups"></a>Come disabilitare i gruppi esterni

La messaggistica esterna di Yammer applica le regole di trasporto di Exchange (ETRs), un insieme di controlli proattivi che impediscono la condivisione delle informazioni aziendali. Per impedire agli utenti di creare gruppi esterni, è necessario configurare una regola di trasporto di Exchange (ETR), quindi configurare Yammer in modo da utilizzare la regola di trasporto di Exchange per bloccare la messaggistica esterna.
  
Dopo aver creato una regola nell'interfaccia di amministrazione di Exchange Online, eseguire la procedura seguente per impostare ETR per l'applicazione in Yammer:
  
- Accedere a Yammer come amministratore verificato e, nell'interfaccia di **amministrazione di Yammer**, passare a impostazioni di ** \> sicurezza di contenuto e** sicurezza di C.

- In **messaggi esterni**selezionare **applica le regole di trasporto di Exchange Online (ETRs) in Yammer.**

- Fare clic su **Salva**.

Per ulteriori informazioni, vedere [controllare la messaggistica esterna in una rete di Yammer con le regole di trasporto di Exchange](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)
  