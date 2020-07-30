---
title: Controllare gli aggiornamenti automatici per le app di Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: 5c56c3adcc9a06db43d4df6f367657cb8ff0c8c8
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 07/28/2020
ms.locfileid: "45431618"
---
# <a name="control-automatic-updates-for-office-apps"></a>Controllare gli aggiornamenti automatici per le app di Office

Per impostazione predefinita, gli aggiornamenti per le app di Office sono scaricati automaticamente e applicati in background senza alcun intervento da parte dell'utente. Tuttavia, gli amministratori possono controllare il modo in cui gli aggiornamenti vengono applicati usando le impostazioni di aggiornamento di Office. Le impostazioni di aggiornamento consentono agli amministratori di abilitare o disabilitare gli aggiornamenti automatici, mostrare o nascondere il pulsante **Aggiorna adesso** in Office, impostare le scadenze degli aggiornamenti e altro ancora. Per informazioni dettagliate, vedere:

- [Configurare le impostazioni di aggiornamento per Office](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [L'aggiornamento automatico per Office non è abilitato](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [Definire la modalità di aggiornamento di Office dopo l'installazione](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

Per controllare le attuali impostazioni degli aggiornamenti applicate a un computer client, eseguire le operazioni seguenti:

1. Aprire l’Editor del Registro di sistema selezionando **Avvio** > **Eseguire** > **regedit**.
2. Passare alla posizione seguente e rivedere le impostazioni di aggiornamento di Office:  
    a. HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office\  
    b. ClickToRun\Configuration

**Nota** Se è impostata la chiave OfficeMgmtCOM, è possibile che venga visualizzato il messaggio "Gli aggiornamenti sono gestiti dall'amministratore di sistema" in **Office** > **Account** > **Aggiornamenti di Office**.  Per altre informazioni, vedere [Gestire gli aggiornamenti di Microsoft 365 Apps con Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).  