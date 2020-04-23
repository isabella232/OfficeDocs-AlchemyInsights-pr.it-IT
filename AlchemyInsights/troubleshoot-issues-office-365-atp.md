---
title: Risoluzione dei problemi relativi a Office 365 Advanced Threat Protection (ATP)
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 99bc985f2d66693aca45f0833ab47c043acc1324
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766749"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a>Risoluzione dei problemi relativi a Office 365 ATP

- **Note ritardi con il recapito dei messaggi di posta elettronica**? Provare a utilizzare l'opzione per il recapito dinamico per i criteri degli allegati sicuri di ATP. In questo modo si eviteranno ritardi nei messaggi di posta elettronica durante la protezione dei destinatari da file dannosi.
- **Si desidera segnalare falsi positivi o falsi negativi**? Utilizzare questo collegamento per inviare il file per l'analisi:[https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)
- Lo sapevate **che è possibile abilitare la protezione dei collegamenti sicuri ATP per la posta elettronica inviata tra gli utenti dell'organizzazione**? Eseguire la procedura seguente:
    1. Vai a https://protection.office.come accedi.
    2. Accedere a**collegamenti attendibili**dei**criteri** > di **gestione delle** > minacce.
    3. In **criteri che si applicano a destinatari specifici**, modificare (o aggiungere) un criterio.
    4. Selezionare **applica collegamenti sicuri ai messaggi inviati all'interno dell'organizzazione**.
    5. Salvare il criterio e consentire circa 30 minuti affinché le modifiche vengano elaborate tramite il Data Center.
- Per ottenere ulteriori informazioni su ATP, vedere [Office 365 Advanced Threat Protection](https://docs.microsoft.com/office365/securitycompliance/office-365-atp).