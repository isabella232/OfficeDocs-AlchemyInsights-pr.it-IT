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
ms.openlocfilehash: e04f8931ef12c426a5c3d5f617fc5f5d5c3a15c6fe43f7b84a7e97e8ee04e3fc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54073964"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-macos-device"></a>Impostare Microsoft Edge come browser predefinito su un dispositivo macOS

Usare uno dei due metodi seguenti per impostare Microsoft Edge come browser predefinito:

Metodo 1: eseguire il flashing del dispositivo con un'immagine macOS in cui Microsoft Edge sia già stato impostato come browser predefinito.

Metodo 2: impostare il criterio DefaultBrowserSettingEnabled per chiedere all'utente di impostare Microsoft Edge come browser predefinito.

Entrambi i metodi consentono a un utente di cambiare il browser predefinito. Per questo motivo, si consiglia di implementare il criterio DefaultBrowserSettingEnabled anche con il metodo 1. Se un utente cambia il browser predefinito dopo aver implementato il criterio, quest'ultimo chiederà all'utente di reimpostare come browser predefinito Microsoft Edge.
