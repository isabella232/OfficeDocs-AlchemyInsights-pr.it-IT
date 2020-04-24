---
title: Dispositivi di Configuration Manager mancanti nel portale
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4384"
ms.openlocfilehash: 7a11ad3c6970be2c52a7cf0696bd3810b9bd665a
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/23/2020
ms.locfileid: "43789906"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a>Dispositivi di Configuration Manager mancanti nel portale

Per il funzionamento della sincronizzazione dei dispositivi, gli [endpoint Internet necessari](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) devono essere raggiungibili dal server locale che ospita il ruolo del punto di connessione del servizio. Per risolvere i problemi di sincronizzazione dei dispositivi, consultare il file **CMGatewaySyncUploadWorker.log** disponibile nel punto di connessione del servizio.

Per altre informazioni, vedere [Collegamento di tenant in Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).
