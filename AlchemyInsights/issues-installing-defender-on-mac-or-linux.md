---
title: Problemi durante l'installazione di Microsoft Defender in Mac o Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: ae17caa4be7809b591be9f9c042186f67828aa3c36a3d17332806e4d92545dc6
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/11/2021
ms.locfileid: "57898612"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a>Problemi durante l'installazione di Microsoft Defender in Mac o Linux

**Mac**

- Verificare che i requisiti di sistema siano soddisfatti prima di installare Microsoft Defender ATP per Mac. Per altre informazioni, vedere [Come installare Microsoft Defender ATP per Mac](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).  
- Rivedere le informazioni nel file: "/Library/Logs/Microsoft/mdatp/install.log".

**Linux**

- Verificare che i requisiti di sistema siano soddisfatti prima di installare Microsoft Defender ATP per Linux. Per altre informazioni, vedere [Come installare MDATP per Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements). 
- Per verificare che il servizio MDATP sia in esecuzione, vedere [Installazione non riuscita](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed).  
    Per risolvere i problemi se il servizio non è in esecuzione, vedere [Procedure per la risoluzione dei problemi se il servizio MDATP non viene eseguito](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running).
- Per la procedura di verifica della configurazione del client, che controlla lo stato di integrità del prodotto, e per eseguire un test di rilevamento nel file di testo EICAR, vedere [Configurazione del client](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).  

    **Nota:** per un elenco dei file system supportati per l’attività di accesso, vedere [Microsoft Defender ATP per Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).