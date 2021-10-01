---
title: Distribuzione di Microsoft 365 Apps per l'utilizzo condiviso in RDS, Terminal Server o VDI
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: ''
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 81183cf1823480c1b15eba9ba9f519b4e3746b52
ms.sourcegitcommit: ef8d6b71fbd962fb3f7081b21724e67a91111a92
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 10/01/2021
ms.locfileid: "60077254"
---
# <a name="deploying-microsoft-365-apps-for-shared-use-on-rds-terminal-server-or-vdi"></a>Distribuzione di Microsoft 365 Apps per l'utilizzo condiviso in RDS, Terminal Server o VDI

Per distribuire Microsoft 365 Apps tramite Servizi Desktop remoto, in precedenza Servizi terminal, è necessario:

- Utilizzare la correzione semplice per abilitare TLS 1.2 come predefinito se si esegue una versione precedente di Windows (ad esempio Windows 7 SP1, Windows Server 2008 R2). Per una correzione semplice e ulteriori informazioni, vedere Aggiornamento per abilitare [TLS 1.1 e TLS 1.2](https://support.microsoft.com/en-us/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392#bkmk_easy)come protocolli sicuri predefiniti in WinHTTP in Windows . 
- Avere un piano che include Microsoft 365 Apps for enterprise (in precedenza Office 365 Plus). Ad esempio, Office 365 E3 o Microsoft 365 E5 o qualsiasi piano che includa la versione desktop di Project o Visio, ad esempio Project - Piano 3 o Visio - Piano 2, o il piano Microsoft 365 Business Premium, che include anche Microsoft 365 Apps for business.
- Abilitare l'attivazione di computer condivisi. Per ulteriori informazioni, vedere [Overview of shared computer activation for Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/overview-shared-computer-activation).

**Nota:** per installare Microsoft 365 Apps in modalità di attivazione di computer condivisi, scaricare ed eseguire [Microsoft Assistente supporto e ripristino](https://aka.ms/SaRA_OfficeSCA_M365Portal). Per informazioni dettagliate sui prerequisiti, le istruzioni di installazione e le istruzioni per personalizzare le installazioni tramite lo strumento di distribuzione di Office, vedere [Deploy Microsoft 365 Apps by using Remote Desktop Services](https://docs.microsoft.com/deployoffice/deploy-microsoft-365-apps-remote-desktop-services).

Per correggere gli errori correlati all'attivazione di computer condivisi, vedere:

- [Risolvere i problemi relativi all'attivazione di computer condivisi per Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation)
- [Reimpostare lo stato di attivazione di Microsoft 365 Apps for enterprise](https://docs.microsoft.com/office/troubleshoot/activation/reset-office-365-proplus-activation-state)

Se si desidera installare Microsoft 365 Apps rds dal interfaccia di amministrazione di Microsoft 365, che utilizza le impostazioni di installazione predefinite, attenersi alla seguente procedura:

1. Controllare il Microsoft 365 piano di cui si dispone. Per ulteriori informazioni, vedere [Quale abbonamento si dispone?](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).

1. Se necessario, passare a un piano Microsoft 365 diverso. Per ulteriori informazioni, vedere [Upgrade to a different plan](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan).

1. Se Microsoft 365 Apps è già installato nel server RDS utilizzando altri piani incompatibili, disinstallarlo andando su **Pannello** di controllo  >  **Disinstallare un programma.** Se si verificano problemi, disinstallare scaricando [Microsoft Assistente supporto e ripristino](https://aka.ms/SARA-OfficeUninstall-Alchemy).

1. Nel server RDS, accedere al interfaccia di amministrazione di Microsoft 365 con l'account di amministratore e [installare Office](https://portal.office.com/OLS/MySoftware.aspx).

   Dopo Office installazione, non aprire o accedere ad alcuna Office applicazioni.

1. Nel server RDS abilitare l'attivazione di computer condivisi modificando il Registro di sistema:

   1. Fai clic con il pulsante Windows pulsante destro del mouse nell'angolo in basso a sinistra dello schermo e scegli **Esegui.** Nella casella Apri digitare **regedit**, quindi fare clic su **OK**.

   1. Quando viene richiesto di consentire all'editor del Registro di sistema di apportare modifiche al dispositivo, selezionare **Sì.**

   1. Nell'editor del Registro di sistema, in HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration, aggiungere un valore stringa **SharedComputerLicensing** con un'impostazione pari a **1.**

1. Nel server RDS, accedere come utente finale e verificare che l'attivazione di computer condivisi sia abilitata per Microsoft 365 Apps. 

   Per informazioni dettagliate, vedere [Verify that shared computer activation is enabled for Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation#verify-that-shared-computer-activation-is-enabled-for-microsoft-365-apps).