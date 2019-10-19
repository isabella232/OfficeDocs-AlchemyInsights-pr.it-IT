---
title: Installazione di Office in un server terminal-senza licenza
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 51d1a66fdf9774bbe58bfdbe89317bc93834be09
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 10/18/2019
ms.locfileid: "37205413"
---
# <a name="installing-office-on-a-terminal-server"></a>Installazione di Office in un server terminal

Per la distribuzione di Office 365 ProPlus in un server Windows utilizzando Servizi Desktop remoto (RDS), precedentemente denominato Servizi terminal:
  
- È necessario disporre di un piano di Office 365 che includa Office 365 ProPlus, ad esempio Office 365 Enterprise E3 o Enterprise E5. I piani di Office 365 business e Office 365 Business Premium non includono Office 365 ProPlus.

- È necessario abilitare l' [attivazione di computer condivisi](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

Se si desidera installare Office 365 ProPlus su RDS dall'interfaccia di amministrazione di Microsoft 365, in ***cui vengono utilizzate le impostazioni di installazione predefinite***, attenersi alla seguente procedura.

> [!TIP]
> È inoltre possibile scaricare ed eseguire l' [Assistente di supporto e ripristino Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) per installare Office 365 ProPlus in modalità di attivazione di computer condivisi.
  
1. Controllare il piano di Office 365. [Informazioni su come](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. Se necessario, passare a un altro piano di Office 365. [Informazioni su come](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. Se Office è già installato nel server RDS utilizzando altri piani di Office 365, disinstallarlo. Ad esempio, accedendo al pannello \> di controllo, disinstallare un programma. Disinstallazione tramite [Assistente di supporto e ripristino di Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) se si è in esecuzione in problemi.

4. Nel server RDS accedere all'interfaccia di amministrazione di Microsoft 365 con l'account di amministratore e [installare Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).

5. Dopo l'installazione di Office, ***non aprire o accedere*** a tutte le applicazioni di Office.

6. Nel server RDS abilitare l'attivazione di computer condivisi modificando il registro di sistema attenendosi alla procedura seguente:

1. Fare clic con il pulsante destro del mouse su Windows nell'angolo in basso a sinistra dello schermo e scegliere Esegui. Nella casella Apri digitare **Regedit**e quindi fare clic su OK.

2. Selezionare Sì quando viene richiesto di consentire all'editor del registro di sistema di apportare modifiche al dispositivo.

3. Nell'editor del registro di sistema, aggiungere un valore stringa di **SharedComputerLicensing** con un'impostazione pari a 1 in HKEY_LOCAL_MACHINE\Software\Microsoft \Office\ClickToRun\Configuration.

7. Nel server RDS, ***accedere come utente finale*** e [verificare che l'attivazione di computer condivisi sia abilitata per Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

Per ulteriori informazioni sui prerequisiti, le istruzioni di installazione e le indicazioni sulle installazioni personalizzate tramite lo strumento di distribuzione di Office, vedere [deploy office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).
  
Per correggere gli errori relativi all'attivazione di computer condivisi, vedere [risolvere i problemi relativi all'attivazione di computer condivisi per Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  