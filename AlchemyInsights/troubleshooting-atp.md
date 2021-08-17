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
ms.openlocfilehash: 484ec1102500b9cce4a1489e016b73e9f73d609e4af95fff13405857d34f3978
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038809"
---
# <a name="troubleshooting-microsoft-defender-for-office-365"></a>Risoluzione dei problemi di Microsoft Defender per Office 365

- **Si nota un ritardo nel recapito dei messaggi?** Usa [l'opzione Recapito](/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) dinamico nel criterio Microsoft Defender per Office 365 Cassaforte allegati. Ciò consente di evitare ritardi nei messaggi proteggendo i destinatari da file dannosi.

- **Si desidera segnalare falsi positivi o falsi negativi a Microsoft?** Usa [Esplora invii](https://protection.office.com/reportsubmission).

-** Si è verificato che è possibile abilitare la protezione dei collegamenti Cassaforte per la posta elettronica interna inviata tra i destinatari all'interno dell'organizzazione?** Attenersi alla seguente procedura:

  1. Accedere a [https://protection.office.com](https://protection.office.com) e accedere con un account amministratore globale o amministratore della sicurezza.

  2. Nel riquadro di spostamento sinistro in **Gestione delle minacce** scegliere Criteri Cassaforte  \> **collegamenti**.

  3. Nella sezione **Criteri applicabili all'intera organizzazione** selezionare il criterio e fare clic su **Modifica.**

  4. In **Impostazioni**, abilitare **Applica collegamenti sicuri ai messaggi inviati all'interno dell'organizzazione**.
