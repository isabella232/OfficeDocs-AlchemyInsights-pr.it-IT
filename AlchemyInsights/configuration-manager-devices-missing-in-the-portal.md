---
title: Dispositivi di Configuration Manager mancanti nel portale
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4384"
ms.openlocfilehash: b6538cb6a348e194856024680a25af948152910a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812155"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a>Dispositivi di Configuration Manager mancanti nel portale

Per il funzionamento della sincronizzazione dei dispositivi, gli [endpoint Internet necessari](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) devono essere raggiungibili dal server locale che ospita il ruolo del punto di connessione del servizio. Per risolvere i problemi di sincronizzazione dei dispositivi, consultare il file **CMGatewaySyncUploadWorker.log** disponibile nel punto di connessione del servizio.

Per altre informazioni, vedere [Collegamento di tenant in Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).
