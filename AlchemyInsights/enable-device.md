---
title: Abilita dispositivo
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "8278"
ms.openlocfilehash: 9e4b03dcba7a2c98a5d63213ee49f9ba8f91d670
ms.sourcegitcommit: 0470a728d184ceb89d1419f7ed57166e07bb778b
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 02/15/2021
ms.locfileid: "50255179"
---
# <a name="enable-device"></a>Abilita dispositivo

**Per abilitare il dispositivo tramite il comando PowerShell**

Eseguire i comandi seguenti:

- Per ottenere l'oggetto dispositivo: `Get-MsolDevice -Name <Name>`
- Per abilitare il dispositivo: `Enable-MsolDevice -DeviceId <DeviceId>`

Per ulteriori informazioni sulla configurazione dell'aggiunta ibrida nei domini gestiti, vedere [Configure Hybrid Join.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains)
