---
title: Errore di licenza DLP di endpoint
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200001"
- "7176"
ms.openlocfilehash: d17c51177898d62c7c477460c8c26b4753bae65f
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/30/2020
ms.locfileid: "49477672"
---
# <a name="endpoint-dlp-licensing-error"></a>Errore di licenza DLP di endpoint

Quando si tenta di configurare l'endpoint DLP, se viene visualizzato un errore seguente:

`Your organization is missing the licenses required to manage these devices`.

Verificare di disporre di una delle sottoscrizioni o dei componenti aggiuntivi seguenti:

- Microsoft 365 E5
- Microsoft 365 A5 (EDU)
- Microsoft 365 E5 Compliance
- Microsoft 365 A5 Compliance
- Microsoft 365 E5 Information Protection and Governance
- Microsoft 365 A5 Information Protection and Governance

> [!NOTE]
> Questa operazione non funzionerà per le combinazioni di licenze quali: Win E5 + O365 E5 + EMS E5. Per impostare questa funzionalità, è necessario disporre di una licenza pura di M365 E5.

Per ulteriori informazioni sulle licenze DLP di endpoint, vedere [Endpoint DLP Licensing.](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)
