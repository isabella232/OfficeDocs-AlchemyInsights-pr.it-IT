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
ms.openlocfilehash: 2dd3c97bb85254215b13ee8a1222941c0492b204
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51806446"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Correzione del messaggio "Non è possibile connettersi subito" alle app di Microsoft 365

Se viene visualizzato questo messaggio, provare a eseguire le operazioni seguenti:

1. Controllare le impostazioni del firewall, del software antivirus e del proxy per verificare che non blocchino l'accesso a Internet alle app di Microsoft 365. Vedere [URL Microsoft e intervalli di indirizzi IP.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Go to **Start**  >  **Run**, and then type **services.msc**. Verificare che tutti i servizi seguenti siano in esecuzione:
    - Configurazione automatica dei dispositivi connessi in rete
    - Servizio elenco di rete
    - Sensibilizzazione percorso di rete
    - Registro eventi di Windows

Se uno di questi servizi non è in esecuzione, provare ad avviarlo. Se si verifica un problema durante l'avvio del servizio, eseguire il comando seguente aprendo un prompt dei comandi con autorizzazioni elevate:

**sfc /scannow**

Al termine del comando, riavviare il computer.

Per informazioni dettagliate, vedere ["Spiacenti, non è possibile connettersi al tuo account. Riprovare più tardi" quando si attiva Office da Microsoft 365.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)