---
title: Risoluzione dei problemi relativi a Office 365 Advanced Threat Protection
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
ms.openlocfilehash: 5a13653ba08d8c6b822354ff70f6d276d31cd816
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658918"
---
# <a name="troubleshooting-office-365-advanced-threat-protection"></a>Risoluzione dei problemi relativi a Office 365 Advanced Threat Protection

- Si notano ritardi nel recapito del messaggio? Utilizzare l'opzione per il [recapito dinamico](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) nel criterio degli allegati sicuri di ATP. In questo modo si eviteranno ritardi nei messaggi proteggendo i destinatari da file dannosi.

- Si desidera segnalare falsi positivi o falsi negativi a Microsoft? Utilizzare questo [collegamento](https://www.microsoft.com/wdsi/filesubmission/) per inviare i file per l'analisi.

- Lo sapevate che è possibile abilitare la protezione dei collegamenti sicuri per la posta elettronica interna inviata tra i destinatari all'interno dell'organizzazione? Eseguire la procedura seguente:

  1. Accedere a [https://protection.office.com](https://protection.office.com) e accedere con un account di amministratore globale o amministratore di sicurezza.

  2. Nel riquadro di spostamento a sinistra in **gestione minacce**scegliere **Policy** \> **collegamenti sicuri**per i criteri.

  3. Nei **criteri che si applicano all'intera sezione organizzazione** selezionare il criterio e fare clic su **modifica**.

  4. In **Impostazioni**, abilitare **applica collegamenti sicuri ai messaggi inviati all'interno dell'organizzazione**.
