---
title: Distribuzione di Microsoft 365 Apps for Enterprise per l'utilizzo condiviso su RDS, Terminal Server o VDI
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: ddd44d40e9430ee31b8b734450dde0defef229d7
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704709"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Distribuzione di Microsoft 365 Apps for Enterprise per l'utilizzo condiviso su RDS, Terminal Server o VDI

Per distribuire le app di Microsoft 365 per Enterprise utilizzando Servizi Desktop remoto (RDS), in precedenza denominato Servizi terminal:
- È necessario disporre di un piano Microsoft 365 per le aziende o di un piano di Office 365 che include le app Microsoft 365 per Enterprise, ad esempio Office 365 Enterprise E3 o Enterprise E5.
   > [!NOTE] 
   > I piani di Microsoft 365 Apps for business e Microsoft 365 Business Premium standard non includono le app Microsoft 365 per Enterprise.
- È necessario abilitare l' [attivazione di computer condivisi](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

> [!NOTE]
> È inoltre possibile scaricare ed eseguire l' [Assistente di supporto e ripristino Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) per installare le app di Microsoft 365 per l'organizzazione in modalità di attivazione di computer condivisi.

Per ulteriori informazioni sui prerequisiti, le istruzioni di installazione e le indicazioni sulle installazioni personalizzate tramite lo strumento di distribuzione di Office, vedere [Deploy Microsoft 365 Apps for Enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).

Per correggere gli errori relativi all'attivazione di computer condivisi:
- Vedere [risolvere i problemi relativi all'attivazione di computer condivisi per le app Microsoft 365 per Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
- Vedere [Reimpostare lo stato di attivazione di Microsoft 365 Apps for enterprise](https://go.microsoft.com/fwlink/?linkid=2109218).

Se si desidera installare le app Microsoft 365 per Enterprise su RDS dall'interfaccia di amministrazione di Microsoft 365, in ***cui vengono utilizzate le impostazioni di installazione predefinite***, attenersi alla procedura seguente:

1.    Controllare la sottoscrizione di cui si dispone. [Procedura](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)
2.    Se necessario, passare a un abbonamento diverso. [Procedura](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)
3.    Se Office è già installato nel server RDS usando altre sottoscrizioni Microsoft, disinstallarlo. Ad esempio, accedendo al **Pannello** > di controllo,**disinstallare un programma**. Disinstallazione tramite [Assistente di supporto e ripristino di Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) se si è in esecuzione in problemi.
4.    Nel server RDS accedere all'interfaccia di amministrazione di Microsoft 365 con l'account di amministratore e [installare le app di microsoft 365 per Enterprise](https://portal.office.com/OLS/MySoftware.aspx).
5.    Dopo l'installazione di Office, ***non aprire o accedere*** a tutte le applicazioni di Office.
6.    Nel server RDS abilitare l'attivazione di computer condivisi modificando il registro di sistema attenendosi alla procedura seguente:
   1. Fare clic con il pulsante destro del mouse su Windows nell'angolo inferiore sinistro dello schermo e scegliere **Esegui**. Nella casella Apri digitare **Regedit**e quindi fare clic su **OK**.
   2. Selezionare **Sì** quando viene richiesto di consentire all'editor del registro di sistema di apportare modifiche al dispositivo.
   3. Nell'editor del registro di sistema, aggiungere un valore stringa di **SharedComputerLicensing** con un'impostazione pari a 1 in HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. Nel server RDS, ***accedere come utente finale*** e [verificare che l'attivazione di computer condivisi sia abilitata per le app Microsoft 365 per Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

