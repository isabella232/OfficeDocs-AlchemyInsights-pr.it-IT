---
title: Risoluzione dei problemi relativi alle app di Microsoft 365, è stato riscontrato un messaggio temporaneo relativo ai server
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: e00504d318efdea4968ddf98b3ce9591f8993e38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758249"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Risoluzione dei problemi relativi alle app Microsoft 365 "dispiaciuti del problema del server temporaneo"

Se viene visualizzato questo messaggio, provare a eseguire le operazioni seguenti:

1. Controllare il firewall, il software antivirus e le impostazioni proxy per confermare che non bloccano l'accesso a Internet alle app Microsoft 365. Vedere [URL e intervalli di indirizzi IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Andare a **Start**  >  **Run**e quindi digitare **Services. msc**. Verificare che i seguenti servizi siano in esecuzione:
    - Configurazione automatica di dispositivi connessi alla rete
    - Servizio elenco di rete
    - Consapevolezza del percorso di rete
    - Registro eventi di Windows

Se uno di questi servizi non è in esecuzione, provare a avviarlo. In caso di problemi durante l'avvio del servizio, eseguire il comando riportato di seguito aprendo un prompt dei comandi con autorizzazioni elevate:

**SFC/scannow**

Al termine del comando, riavviare il computer.

Per informazioni dettagliate, vedere [la sezione "spiacenti, non è possibile connettersi al proprio account. Si prega di riprovare più tardi "errore quando si attiva](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).