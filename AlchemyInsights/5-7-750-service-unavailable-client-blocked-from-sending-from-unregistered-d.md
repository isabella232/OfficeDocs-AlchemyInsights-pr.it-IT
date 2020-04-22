---
title: 1048 servizio 5.7.750 non disponibile. Client bloccato dall'invio di domini non registrati
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom:
- "1048"
- "3100026"
ms.openlocfilehash: 48b9c2de27f8d7f52215c3a3d547bdf746a3a4cd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676717"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a>5.7.750 Al client è impedito l'invio da un dominio non registrato

L'errore si verifica quando un numero elevato di messaggi viene inviato da domini non sottoposto a provisioning nel tenant (aggiunti come domini accettati e convalidati).

Per evitare questo errore, è possibile utilizzare un connettore del flusso di posta basato sui certificati in cui il dominio del certificato è un dominio di cui è stato effettuato il provisioning oppure eseguire il provisioning di tutti i domini di invio.
