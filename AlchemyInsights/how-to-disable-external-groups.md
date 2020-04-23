---
title: Come disabilitare i gruppi esterni
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 2159feb4aa3999072de57d76790a2959c7355976
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720772"
---
# <a name="how-to-disable-external-groups"></a>Come disabilitare i gruppi esterni

La messaggistica esterna di Yammer applica le regole di trasporto di Exchange (ETRs), un insieme di controlli proattivi che impediscono la condivisione delle informazioni aziendali. Per impedire agli utenti di creare gruppi esterni, è necessario configurare una regola di trasporto di Exchange (ETR), quindi configurare Yammer in modo da utilizzare la regola di trasporto di Exchange per bloccare la messaggistica esterna.
  
Dopo aver creato una regola nell'interfaccia di amministrazione di Exchange Online, eseguire la procedura seguente per impostare ETR per l'applicazione in Yammer:
  
- Accedere a Yammer come amministratore verificato e, nell'interfaccia di **amministrazione di Yammer**, passare a impostazioni di ** \> sicurezza di contenuto e** sicurezza di C.

- In **messaggi esterni**selezionare **applica le regole di trasporto di Exchange Online (ETRs) in Yammer.**

- Fare clic su **Salva**.

Per ulteriori informazioni, vedere [Disable External Messaging in a Yammer Network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).
  