---
title: Risoluzione dei problemi di Microsoft Defender per Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: 91d73853d3ea67d6c6954fffb32dd1428e3d9976
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545272"
---
# <a name="troubleshooting-microsoft-defender-for-office-365"></a>Risoluzione dei problemi di Microsoft Defender per Office 365

- **Si nota un ritardo nel recapito dei messaggi?** Usa [l'opzione Recapito](/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) dinamico in Microsoft Defender per Office 365 allegati sicuri. Ciò consente di evitare ritardi nei messaggi proteggendo i destinatari da file dannosi.

- **Si desidera segnalare falsi positivi o falsi negativi a Microsoft?** Usa [Esplora invii](https://protection.office.com/reportsubmission).

-** Si è verificato che è possibile abilitare la protezione dei collegamenti sicuri per la posta elettronica interna inviata tra destinatari all'interno dell'organizzazione?** Eseguire la procedura seguente:

  1. Accedere a [https://protection.office.com](https://protection.office.com) e accedere con un account amministratore globale o amministratore della sicurezza.

  2. Nel riquadro di spostamento a sinistra in **Gestione delle minacce** scegliere Collegamenti **sicuri** per i \> **criteri.**

  3. Nella sezione **Criteri applicabili all'intera organizzazione** selezionare il criterio e fare clic su **Modifica.**

  4. In **Impostazioni**, abilitare **Applica collegamenti sicuri ai messaggi inviati all'interno dell'organizzazione**.
