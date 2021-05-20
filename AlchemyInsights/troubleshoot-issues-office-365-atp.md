---
title: Risolvere i problemi con Microsoft Defender per Office 365
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: d6170ac52b9af4d2bc6f8822ff2a9b8c1b161ed9
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544762"
---
# <a name="troubleshoot-issues-with-microsoft-defender-for-office-365"></a>Risolvere i problemi con Microsoft Defender per Office 365

- **Si notino ritardi con il recapito dei messaggi di posta elettronica**? Prova a usare l'opzione Recapito dinamico per Microsoft Defender per i criteri Office 365 allegati sicuri. In questo modo si evitano ritardi nel recapito dei messaggi di posta elettronica proteggendo i destinatari da file dannosi.
- **Si desidera segnalare falsi positivi o falsi negativi?** Usa [Esplora invii](https://protection.office.com/reportsubmission).
- Si sa che è possibile abilitare Microsoft Defender per Microsoft Defender per Office 365 protezione dei collegamenti sicuri per la posta elettronica inviata tra persone **dell'organizzazione?** Eseguire la procedura seguente:
    1. Vai a https://protection.office.com e accedi.
    2. Passare a **Criteri di gestione**  >  **delle** minacce Collegamenti  >  **sicuri**.
    3. In **Criteri applicabili a destinatari specifici** modificare o aggiungere un criterio.
    4. Selezionare **Applica collegamenti sicuri ai messaggi inviati all'interno dell'organizzazione.**
    5. Salvare i criteri e consentire fino a 30 minuti per l'applicazione delle modifiche.

- Per altre informazioni su Microsoft Defender per Office 365, vedi [Microsoft Defender per Office 365](/microsoft-365/security/office-365-security/office-365-atp).