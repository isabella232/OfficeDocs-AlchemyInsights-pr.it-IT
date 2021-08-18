---
title: Installazione di Office in un server terminal - Senza licenza
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 35ef317ea87fedd01c08fee5b370e3c81e515c27
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58322003"
---
# <a name="installing-office-on-a-terminal-server"></a>Installazione di Office in un server terminal

Per la distribuzione Microsoft 365 Apps for enterprise in un Windows Server tramite Servizi Desktop remoto, in precedenza denominato Servizi terminal:
  
- È necessario disporre di una sottoscrizione Microsoft 365 che includa Microsoft 365 Apps for enterprise, ad esempio Office 365 Enterprise E3 o Enterprise E5. I Microsoft 365 Apps for business e Microsoft 365 Apps for business Premium non includono Microsoft 365 Apps for enterprise.

- È necessario abilitare [l'attivazione di computer condivisi](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

Se si desidera installare Microsoft 365 Apps for enterprise in RDS dal ***interfaccia di amministrazione di Microsoft 365,*** che utilizza le impostazioni di installazione predefinite, eseguire la procedura seguente.

    **Tip**: You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.
  
1. Controlla l Microsoft 365 abbonamento che hai. [Altre informazioni](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. Se necessario, passare a un abbonamento Microsoft 365 diverso. [Altre informazioni](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Se Office è già installato nel server RDS utilizzando altre sottoscrizioni Microsoft 365, disinstallarlo. Ad esempio, andando a Pannello di controllo \> Disinstallare un programma. Disinstallare [usando Microsoft Assistente supporto e ripristino](https://aka.ms/SARA-OfficeUninstall-Alchemy) se si verificano problemi.

4. Nel server RDS, accedere al interfaccia di amministrazione di Microsoft 365 con l'account di amministratore e [installare Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).

5. Dopo Office installazione, non aprire o accedere ***ad*** alcuna Office applicazioni.

6. Nel server RDS abilitare l'attivazione di computer condivisi modificando il Registro di sistema seguendo questa procedura:

1. Fai clic con il pulsante Windows clic con il pulsante destro del mouse sul pulsante Windows nell'angolo in basso a sinistra dello schermo e scegli Esegui. Nella casella Apri digitare **regedit** e quindi selezionare OK.

2. Selezionare Sì quando viene richiesto di consentire all'editor del Registro di sistema di apportare modifiche al dispositivo.

3. Nell'editor del Registro di sistema aggiungi un valore stringa **SharedComputerLicensing** con un'impostazione pari a 1 in HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. Nel server RDS, ***accedere come utente*** finale e verificare che l'attivazione di computer condivisi sia abilitata per [Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

Per ulteriori informazioni sui prerequisiti, sulle istruzioni di installazione e sulle istruzioni per le installazioni personalizzate tramite lo strumento di distribuzione di Office, vedere [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).
  
Per correggere gli errori correlati all'attivazione di computer condivisi, vedere Risolvere i problemi relativi all'attivazione di computer condivisi [per Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
  