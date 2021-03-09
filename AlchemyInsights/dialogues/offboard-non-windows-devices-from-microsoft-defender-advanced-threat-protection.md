---
title: Offboard dei dispositivi non Windows da Microsoft Defender Advanced Threat Protection (ATP)
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
ms.openlocfilehash: 435957c555cd80155a985a49bd94b041a4ada31d
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/08/2021
ms.locfileid: "50530219"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a>Offboard dei dispositivi non Windows da Microsoft Defender Advanced Threat Protection (ATP)

Ecco come:

1. Seguire la documentazione di terze parti per disconnettere la soluzione di terze parti da Microsoft Defender ATP.
2. Dal tenant di Azure Active Directory, rimuovere le autorizzazioni per la soluzione di terze parti:

    1. Accedere al [portale di Azure](https://go.microsoft.com/fwlink/?linkid=2125612).
    1. Selezionare **Tutti i servizi** Azure Active  >  **Directory** Enterprise  >  **Applications.**
    1. Seleziona l'applicazione che vuoi eseguire l'offboard.
    1. Selezionare **Elimina**.

Per altre informazioni, vedi [Eseguire l'offboard dei dispositivi non Windows.](https://go.microsoft.com/fwlink/?linkid=2143630)
