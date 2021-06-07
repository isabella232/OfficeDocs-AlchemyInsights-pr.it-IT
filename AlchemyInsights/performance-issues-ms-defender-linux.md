---
title: Problemi di prestazioni per Microsoft Defender per endpoint su Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 06/06/2021
ms.locfileid: "52783433"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a>Problemi di prestazioni per Microsoft Defender per endpoint su Linux

In questo articolo vengono specificati i passaggi per l'identificazione dei problemi di prestazioni per Microsoft Defender per endpoint su Linux.

Per prima cosa, è importante verificare se problema riscontrato sia risolvibile nella [versione più recente](/microsoft-365/security/defender-endpoint/linux-whatsnew). 

Per avviare l'indagine, vedere [Risoluzione dei problemi di prestazioni per Microsoft Defender per endpoint su Linux](/microsoft-365/security/defender-endpoint/linux-support-perf).

## <a name="exclusions"></a>Esclusioni

Le esclusioni possono aiutare a ridurre i problemi di prestazioni. Rivedere le esclusioni prima di iniziare, così che qualsiasi rischio aggiuntivo sia noto e documentato.

Per ulteriori informazioni, vedere [Configurare e convalidare le esclusioni per Microsoft Defender per endpoint su Linux](/microsoft-365/security/defender-endpoint/linux-exclusions).

Se si dispone di più file e cartelle da escludere sullo stesso punto di montaggio, potrebbe essere più facile escludere tale punto di montaggio. A partire dalla release 101.22.80 di febbraio, è possibile escludere un intero punto di montaggio.

Ad esempio, se /mnt/backup è un punto di montaggio, è possibile aggiungere /mnt/backup all'elenco di esclusione eseguendo questo domando:

`$ mdatp exclusion folder add –path /mnt/backup`

**Nota**: l'aggiunta di esclusioni aumenta il rischio della mancata identificazione di malware e dovrebbe essere gestita e implementata con attenzione.

## <a name="need-help"></a>Servono altre informazioni?

Per poter ricevere la migliore assistenza, è necessario fornire i dati di diagnostica prima di aprire un caso di supporto.
