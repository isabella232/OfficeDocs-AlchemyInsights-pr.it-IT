---
title: 'Problema di attivazione: non è possibile connettersi in questo momento'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 56accf68f2cf41dbe6119281b74e2cb56b702789
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716176"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a>Risoluzione delle app di Office "non è possibile connettersi subito" messaggio

Se viene visualizzato questo messaggio, provare a eseguire le operazioni seguenti:

1. Controllare il firewall, il software antivirus e le impostazioni proxy per confermare che non bloccano l'accesso a Internet alle app di Office. Vedere gli [intervalli di indirizzi IP e URL Microsoft](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Andare a **Start** > **Run**e quindi digitare **Services. msc**. Verificare che i seguenti servizi siano in esecuzione:
    - Configurazione automatica di dispositivi connessi alla rete
    - Servizio elenco di rete
    - Consapevolezza del percorso di rete
    - Registro eventi di Windows

Se uno di questi servizi non è in esecuzione, provare a avviarlo. In caso di problemi durante l'avvio del servizio, eseguire il comando riportato di seguito aprendo un prompt dei comandi con autorizzazioni elevate:

**SFC/scannow**

Al termine del comando, riavviare il computer.

Per informazioni dettagliate, vedere [la sezione "spiacenti, non è possibile connettersi al proprio account. Si prega di riprovare più tardi quando si attiva Office da Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).