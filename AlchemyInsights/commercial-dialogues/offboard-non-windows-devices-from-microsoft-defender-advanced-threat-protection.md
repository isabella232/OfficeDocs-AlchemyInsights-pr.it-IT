---
title: Offboard non Windows dispositivi da Microsoft Defender Advanced Threat Protection (ATP)
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: fbaab348e06691b73db68492a0083c4a5a54c4504e03d27ec53f2a9f5047266d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53967805"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a>Offboard non Windows dispositivi da Microsoft Defender Advanced Threat Protection (ATP)

Ecco come:

1. Seguire la documentazione di terze parti per disconnettere la soluzione di terze parti da Microsoft Defender ATP.
2. Dal tenant Azure Active Directory, rimuovere le autorizzazioni per la soluzione di terze parti:

    1. Accedere al [portale di Azure](https://go.microsoft.com/fwlink/?linkid=2125612).
    1. Selezionare **Tutti i servizi**  >  **Azure Active Directory** Enterprise  >  **applicazioni**.
    1. Seleziona l'applicazione che vuoi offboard.
    1. Selezionare **Elimina**.

Per altre informazioni, vedi [Offboard non Windows dispositivi](https://go.microsoft.com/fwlink/?linkid=2143630).
