---
title: Endpoint DLP licensing error
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
ms.openlocfilehash: c32ab88a72c265be411350e50756f5b2e1e3337c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58322135"
---
# <a name="endpoint-dlp-licensing-error"></a>Endpoint DLP Licensing error

Quando si tenta di configurare Endpoint DLP, se viene visualizzato il seguente errore:

`Your organization is missing the licenses required to manage these devices`.

Verificare di disporre di una delle sottoscrizioni o dei componenti aggiuntivi seguenti:

- Microsoft 365 E5
- Microsoft 365 A5 (EDU)
- Microsoft 365 E5 Compliance
- Microsoft 365 A5 Compliance
- Microsoft 365 E5 Information Protection and Governance
- Microsoft 365 A5 Information Protection and Governance

**Nota:** non funziona per combinazioni di licenze come: Win E5 + O365 E5 + EMS E5. Per configurare questa funzionalità, è necessario disporre di una licenza M365 E5 pura.

Per altre informazioni sulle licenze di Endpoint DLP, vedi [Endpoint DLP Licensing.](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)
