---
title: Correzione di Microsoft 365 app Spiacenti, si sta verificando un messaggio di problemi temporanei del server
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
- "3420"
- "9001430"
ms.openlocfilehash: 565f70d9a09c61bef84cdd1c23e9b0ed34bebe51
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744671"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Correzione del messaggio Microsoft 365 app "Spiacenti, si sono verificati problemi temporanei del server"

Nota: se si utilizza una versione precedente di Windows (ad esempio Windows 7 SP1, Windows Server 2008 [](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) R2), utilizzare la correzione semplice per abilitare TLS 1.2 come predefinito. Per ulteriori informazioni, vedere [Aggiornamento per abilitare TLS 1.1 e TLS 1.2 come protocollo di protezione predefinito in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).

Se viene visualizzato questo messaggio, provare a eseguire le operazioni seguenti:

1. Controlla le impostazioni del firewall, del software antivirus e del proxy per verificare che non blocchino l'accesso a Internet Microsoft 365 app. Vedere [URL e intervalli di indirizzi IP.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Go to **Start**  >  **Run**, and then type **services.msc**. Verificare che tutti i servizi seguenti siano in esecuzione:
    - Configurazione automatica dei dispositivi connessi in rete
    - Servizio elenco di rete
    - Sensibilizzazione percorso di rete
    - Registro eventi di Windows

Se uno di questi servizi non è in esecuzione, provare ad avviarlo. Se si verifica un problema durante l'avvio del servizio, eseguire il comando seguente aprendo un prompt dei comandi con autorizzazioni elevate:

**sfc /scannow**

Al termine del comando, riavviare il computer.

Per informazioni dettagliate, vedere ["Spiacenti, non è possibile connettersi al tuo account. Riprovare più tardi" quando si attiva](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).