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
ms.openlocfilehash: 6646ca4792ac4d9fb8bfb7433d53ecf4aeba8da0aca797225c16c02b28499889
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013248"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a>Problemi durante l'installazione di Microsoft Defender in Mac o Linux

**Mac**

- Verificare che i requisiti di sistema siano soddisfatti prima di installare Microsoft Defender ATP per Mac. Per altre informazioni, vedere [Come installare Microsoft Defender ATP per Mac](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).  
- Rivedere le informazioni nel file: "/Library/Logs/Microsoft/mdatp/install.log".

**Linux**

- Verificare che i requisiti di sistema siano soddisfatti prima di installare Microsoft Defender ATP per Linux. Per altre informazioni, vedere [Come installare MDATP per Linux](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements). 
- Per verificare che il servizio MDATP sia in esecuzione, vedere [Installazione non riuscita](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed).  
    Per risolvere i problemi se il servizio non è in esecuzione, vedere [Procedure per la risoluzione dei problemi se il servizio MDATP non viene eseguito](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running).
- Per la procedura di verifica della configurazione del client, che controlla lo stato di integrità del prodotto, e per eseguire un test di rilevamento nel file di testo EICAR, vedere [Configurazione del client](/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).  

    **Nota:** per un elenco dei file system supportati per l’attività di accesso, vedere [Microsoft Defender ATP per Linux](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).