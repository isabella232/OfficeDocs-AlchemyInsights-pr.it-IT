---
title: Come disabilitare i gruppi esterni
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 9c513da49dc953b4ae76bb06854e33232ec40e11151f11ade33c3080092aa598
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54015624"
---
# <a name="how-to-disable-external-groups"></a>Come disabilitare i gruppi esterni

Yammer messaggistica esterna si applica Exchange Transport Rules (ETR), un set di controlli proattivi per impedire la condivisione delle informazioni aziendali. Per impedire agli utenti di creare gruppi esterni, è necessario configurare una regola di trasporto Exchange e quindi configurare Yammer per l'utilizzo della regola di trasporto Exchange per bloccare la messaggistica esterna.
  
Dopo aver creato una regola nell'Exchange Online di amministrazione, eseguire la procedura seguente per impostare ETR per l'applicazione in Yammer:
  
- Accedere a Yammer come amministratore verificato e nell'interfaccia di amministrazione di **Yammer** passare a Contenuto C e sicurezza **\> Impostazioni.**

- In **Messaggistica esterna** selezionare Imponi regole di trasporto **Exchange Online Exchange (ETR) in Yammer.**

- Scegliere **Salva**.

Per ulteriori informazioni, vedere [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).
  