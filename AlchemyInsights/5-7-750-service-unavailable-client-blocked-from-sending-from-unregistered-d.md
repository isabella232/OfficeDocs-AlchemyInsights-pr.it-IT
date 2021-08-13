---
title: 1048 5.7.750 Servizio non disponibile. Client bloccato dall'invio da domini non registrati
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom:
- "1048"
- "3100026"
ms.openlocfilehash: 0fd0fd730d562fa0313d61c1593d6eab91b3bc8cc15ba277e9cd4e4deb6901bd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53919067"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a>5.7.750 Al client è impedito l'invio da un dominio non registrato

L'errore si verifica quando un volume elevato di messaggi viene inviato da domini di cui non è stato eseguito il provisioning nel tenant (aggiunti come domini accettati e convalidati).

Per evitare questo errore, è possibile utilizzare un connettore del flusso di posta basato su certificato in cui il dominio del certificato è un dominio di cui è stato eseguito il provisioning oppure è possibile eseguire il provisioning di tutti i domini di invio.

Per altre informazioni, vedere [Risolvere i problemi di recapito della posta elettronica per i codici di errore da 5.7.700 a 5.7.750 in Exchange Online](https://go.microsoft.com/fwlink/?linkid=2164955).