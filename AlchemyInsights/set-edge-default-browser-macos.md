---
title: Impostare Microsoft Edge come browser predefinito su un dispositivo macOS
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: 5318c7d20ee7091e162e566cd2b4ebf5d255915b
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426820"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-macos-device"></a>Impostare Microsoft Edge come browser predefinito su un dispositivo macOS

Usare uno dei due metodi seguenti per impostare Microsoft Edge come browser predefinito:

Metodo 1: eseguire il flashing del dispositivo con un'immagine macOS in cui Microsoft Edge sia già stato impostato come browser predefinito.

Metodo 2: impostare il criterio DefaultBrowserSettingEnabled per chiedere all'utente di impostare Microsoft Edge come browser predefinito.

Entrambi i metodi consentono a un utente di cambiare il browser predefinito. Per questo motivo, si consiglia di implementare il criterio DefaultBrowserSettingEnabled anche con il metodo 1. Se un utente cambia il browser predefinito dopo aver implementato il criterio, quest'ultimo chiederà all'utente di reimpostare come browser predefinito Microsoft Edge.
