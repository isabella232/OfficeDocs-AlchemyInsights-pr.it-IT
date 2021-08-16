---
title: Distribuzione di Microsoft 365 Apps for enterprise per l'utilizzo condiviso in RDS, Terminal Server o VDI
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
ms.openlocfilehash: 55b86557ec205dde2c459d76e8e330d2a8271dbec723f079e119ebe409b41c3f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54031482"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Distribuzione di Microsoft 365 Apps for enterprise per l'utilizzo condiviso in RDS, Terminal Server o VDI

Per distribuire Microsoft 365 Apps for enterprise tramite Servizi Desktop remoto, in precedenza denominato Servizi terminal:

- È necessario disporre di un piano Microsoft 365 For Business o di un piano di Office 365 che includa Microsoft 365 Apps for enterprise, ad esempio Office 365 Enterprise E3 o Enterprise E5.
   > [!NOTE]
   > I Microsoft 365 Apps for business e Microsoft 365 Business Standard non includono Microsoft 365 Apps for enterprise.
- È necessario abilitare [l'attivazione di computer condivisi](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

> [!NOTE]
> È inoltre possibile scaricare ed eseguire [Microsoft Assistente supporto e ripristino](https://aka.ms/SaRA_OfficeSCA_M365Portal) per installare Microsoft 365 Apps for enterprise in modalità di attivazione di computer condivisi.

Per ulteriori informazioni sui prerequisiti, le istruzioni di installazione e le indicazioni sulle installazioni personalizzate tramite lo strumento di distribuzione di Office, vedere [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).

Per correggere gli errori correlati all'attivazione di computer condivisi:

- Vedi [Risolvere i problemi relativi all'attivazione di computer condivisi per Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
- Vedere [Reimpostare lo stato di attivazione di Microsoft 365 Apps for enterprise](https://go.microsoft.com/fwlink/?linkid=2109218).

Se si desidera installare Microsoft 365 Apps for enterprise in RDS dalla ***interfaccia di amministrazione di Microsoft 365,*** che utilizza le impostazioni di installazione predefinite, eseguire la procedura seguente:

1. Controlla quale abbonamento hai. [Procedura](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)
2. Se necessario, passare a un abbonamento diverso. [Procedura](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)
3. Se Office è già installato nel server RDS utilizzando altre sottoscrizioni Microsoft, disinstallarlo. Ad esempio, andando a **Pannello di controllo**  >  **Disinstallare un programma**. Disinstallare [usando Microsoft Assistente supporto e ripristino](https://aka.ms/SARA-OfficeUninstall-Alchemy) se si verificano problemi.
4. Nel server RDS, accedere al interfaccia di amministrazione di Microsoft 365 con l'account di amministratore e [installare Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).
5. Dopo Office installazione, non aprire o accedere ***ad*** alcuna Office applicazioni.
6. Nel server RDS abilitare l'attivazione di computer condivisi modificando il Registro di sistema seguendo questa procedura:
   1. Fai clic con il pulsante Windows pulsante destro del mouse nell'angolo in basso a sinistra dello schermo e scegli **Esegui.** Nella casella Apri digitare **regedit**, quindi fare clic su **OK**.
   2. Selezionare **Sì** quando viene richiesto di consentire all'editor del Registro di sistema di apportare modifiche al dispositivo.
   3. Nell'editor del Registro di sistema aggiungi un valore stringa **SharedComputerLicensing** con un'impostazione pari a 1 in HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. Nel server RDS, ***accedere come utente finale*** e verificare che l'attivazione di computer condivisi sia [abilitata per Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).
