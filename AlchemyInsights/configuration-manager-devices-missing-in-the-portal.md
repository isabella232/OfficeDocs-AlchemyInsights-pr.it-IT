---
title: Dispositivi di Configuration Manager mancanti nel portale
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4384"
ms.openlocfilehash: d57659eb928dd8c4653499e65b6e6cd2f021f521
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817248"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a>Dispositivi di Configuration Manager mancanti nel portale

Per il funzionamento della sincronizzazione dei dispositivi, gli [endpoint Internet necessari](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) devono essere raggiungibili dal server locale che ospita il ruolo del punto di connessione del servizio. Per risolvere i problemi di sincronizzazione dei dispositivi, consultare il file **CMGatewaySyncUploadWorker.log** disponibile nel punto di connessione del servizio.

Per altre informazioni, vedere [Collegamento di tenant in Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).
