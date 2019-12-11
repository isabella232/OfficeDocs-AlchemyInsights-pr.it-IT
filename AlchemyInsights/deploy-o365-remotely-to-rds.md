---
title: Distribuzione di Office 365 ProPlus per l'utilizzo condiviso su RDS, Terminal Server o VDI
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 12/9/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 2312cca9ebf5dad1322bc98335cef6a6bc81f03e
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959464"
---
# <a name="deploying-office-365-proplus-for-shared-use-on-rds-terminal-server-or-vdi"></a>Distribuzione di Office 365 ProPlus per l'utilizzo condiviso su RDS, Terminal Server o VDI

Per distribuire Office 365 ProPlus utilizzando Servizi Desktop remoto (RDS), in precedenza denominati Servizi terminal:
- È necessario disporre di un piano Microsoft 365 per le aziende o di un piano di Office 365 che include Office 365 ProPlus, ad esempio Office 365 Enterprise E3 o Enterprise E5.
   > [!NOTE] 
   > I piani di Office 365 business e Office 365 Business Premium non includono Office 365 ProPlus.
- È necessario abilitare l' [attivazione di computer condivisi](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

> [!NOTE]
> È inoltre possibile scaricare ed eseguire l' [Assistente di supporto e ripristino Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) per installare Office 365 ProPlus in modalità di attivazione di computer condivisi.

Per ulteriori informazioni sui prerequisiti, le istruzioni di installazione e le indicazioni sulle installazioni personalizzate tramite lo strumento di distribuzione di Office, vedere [deploy office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).

Per correggere gli errori relativi all'attivazione di computer condivisi:
- Vedere [risolvere i problemi relativi all'attivazione di computer condivisi per Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
- Vedere [reimpostare lo stato di attivazione di Office 365 ProPlus](https://go.microsoft.com/fwlink/?linkid=2109218).

Se si desidera installare Office 365 ProPlus su RDS dall'interfaccia di amministrazione di Microsoft 365, in ***cui vengono utilizzate le impostazioni di installazione predefinite***, attenersi alla procedura seguente:

1.  Controllare il piano di Office 365. [Procedura](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)
2.  Se necessario, passare a un altro piano di Office 365. [Procedura](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)
3.  Se Office è già installato nel server RDS utilizzando altri piani di Office 365, disinstallarlo. Ad esempio, accedendo al **Pannello** > di controllo,**disinstallare un programma**. Disinstallazione tramite [Assistente di supporto e ripristino di Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) se si è in esecuzione in problemi.
4.  Nel server RDS accedere all'interfaccia di amministrazione di Microsoft 365 con l'account di amministratore e [installare Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).
5.  Dopo l'installazione di Office, ***non aprire o accedere*** a tutte le applicazioni di Office.
6.  Nel server RDS abilitare l'attivazione di computer condivisi modificando il registro di sistema attenendosi alla procedura seguente:
   1. Fare clic con il pulsante destro del mouse su Windows nell'angolo inferiore sinistro dello schermo e scegliere **Esegui**. Nella casella Apri digitare **Regedit**e quindi fare clic su **OK**.
   2. Selezionare **Sì** quando viene richiesto di consentire all'editor del registro di sistema di apportare modifiche al dispositivo.
   3. Nell'editor del registro di sistema, aggiungere un valore stringa di **SharedComputerLicensing** con un'impostazione pari a 1 in HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. Nel server RDS, ***accedere come utente finale*** e [verificare che l'attivazione di computer condivisi sia abilitata per Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

