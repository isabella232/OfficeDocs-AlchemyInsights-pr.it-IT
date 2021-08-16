---
title: 'Problema di attivazione: al momento non è possibile connettersi'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 5dad4b43efac2468b57351a4d6c96379ed505071ca144ec0aa518e975633bb18
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998159"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Correzione del messaggio Microsoft 365 app "Non è possibile connettersi al momento"

Se viene visualizzato questo messaggio, provare a eseguire le operazioni seguenti:

1. Controlla le impostazioni del firewall, del software antivirus e del proxy per verificare che non blocchino l'accesso a Internet Microsoft 365 app. Vedere [URL Microsoft e intervalli di indirizzi IP.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Go to **Start**  >  **Run**, and then type **services.msc**. Verificare che tutti i servizi seguenti siano in esecuzione:
    - Configurazione automatica dei dispositivi connessi in rete
    - Servizio elenco di rete
    - Sensibilizzazione percorso di rete
    - Registro eventi di Windows

Se uno di questi servizi non è in esecuzione, provare ad avviarlo. Se si verifica un problema durante l'avvio del servizio, eseguire il comando seguente aprendo un prompt dei comandi con autorizzazioni elevate:

**sfc /scannow**

Al termine del comando, riavviare il computer.

Per informazioni dettagliate, vedere ["Spiacenti, non è possibile connettersi al tuo account. Riprovare più tardi" quando si](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)attiva Office da Microsoft 365 .