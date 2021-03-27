---
title: Accedere a Microsoft Edge manualmente
ms.author: v-smandalika
author: v-smandalika
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9003844"
- "6893"
- "8332"
- "9004625"
ms.openlocfilehash: f380d09dc14788205638cdee6aebe0b084ecab2f
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398661"
---
# <a name="sign-in-to-microsoft-edge-manually"></a>Accedere a Microsoft Edge manualmente

Se un utente non è connesso automaticamente durante un'esperienza di prima esecuzione, l'utente può accedere manualmente tramite le impostazioni del browser o il riquadro a comparsa dell'identità. Per gestire l'accesso, utilizzare i criteri seguenti:

1. [NonRemovableProfileEnabled](https://docs.microsoft.com/deployedge/microsoft-edge-policies#nonremovableprofileenabled) - Per garantire che un utente abbia sempre un profilo di lavoro in Microsoft Edge.
2. [RestrictSigninToPattern](https://docs.microsoft.com/deployedge/microsoft-edge-policies#restrictsignintopattern) - Per limitare l'accesso a un set di account attendibili.
3. [BrowserSignin:](https://docs.microsoft.com/deployedge/microsoft-edge-policies#browsersignin) per disabilitare l'accesso o per forzare l'accesso degli utenti.

