---
title: Risoluzione dei problemi relativi a Microsoft Defender per Office 365
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
ms.openlocfilehash: 2c9543660056ebc02b0bd297f619f20fa6820093
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801447"
---
# <a name="troubleshooting-microsoft-defender-for-office-365"></a>Risoluzione dei problemi relativi a Microsoft Defender per Office 365

- Si notano ritardi nel recapito del messaggio? Utilizzare l'opzione per il [recapito dinamico](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) nel criterio degli allegati sicuri di ATP. In questo modo si eviteranno ritardi nei messaggi proteggendo i destinatari da file dannosi.

- Si desidera segnalare falsi positivi o falsi negativi a Microsoft? Utilizzare questo [collegamento](https://www.microsoft.com/wdsi/filesubmission/) per inviare i file per l'analisi.

- Lo sapevate che è possibile abilitare la protezione dei collegamenti sicuri per la posta elettronica interna inviata tra i destinatari all'interno dell'organizzazione? attenersi alla seguente procedura:

  1. Accedere a [https://protection.office.com](https://protection.office.com) e accedere con un account di amministratore globale o amministratore di sicurezza.

  2. Nel riquadro di spostamento a sinistra in **gestione minacce** scegliere **Policy** \> **collegamenti sicuri** per i criteri.

  3. Nei **criteri che si applicano all'intera sezione organizzazione** selezionare il criterio e fare clic su **modifica** .

  4. In **Impostazioni** , abilitare **applica collegamenti sicuri ai messaggi inviati all'interno dell'organizzazione** .
