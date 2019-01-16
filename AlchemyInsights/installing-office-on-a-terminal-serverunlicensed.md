---
title: Installazione di office in un Server Terminal - senza licenza
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 73d5128b55cae7712c48be9e2d05e558c3ba2e5c
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/15/2019
ms.locfileid: "28296520"
---
# <a name="installing-office-on-a-terminal-server"></a>Installazione di Office in un Server Terminal

Per la distribuzione di Office 365 ProPlus in Windows Server tramite Servizi Desktop remoto (RDS), denominato in precedenza Servizi Terminal:
  
- È necessario disporre di un piano di Office 365 che include Office 365 ProPlus, ad esempio Office 365 Enterprise E3 o E5 Enterprise. Piani di Office 365 Business e di Office 365 Business Premium non includono Office 365 ProPlus.
    
- È necessario abilitare [l'attivazione di computer condiviso](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).
    
Se si desidera installare Office 365 ProPlus in RDS dal portale di Office 365, * * *che utilizza le impostazioni di installazione predefinito* * *, eseguire la procedura seguente: 
  
1. Controllare il piano di Office 365 si dispone. [Informazioni su come](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)
    
2. Se necessario, passare a un altro di Office 365 prevede. [Informazioni su come](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)
    
3. Se Office è già installato nel server RDS con altri piani di Office 365, è necessario disinstallarlo. Ad esempio, passando al pannello di controllo \> Disinstalla un programma. Disinstallare tramite [Assistente di ripristino e supporto tecnico clienti Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) se si esegue problemi. 
    
4. In server RDS, accedere al portale di Office 365 con il proprio account di amministratore e [installare Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).
    
5. Dopo l'installazione di Office, * * *non aprire o accedere* * * per tutte le applicazioni di Office. 
    
6. Nel server RDS, abilitare l'attivazione di computer condiviso modificando il Registro di sistema eseguendo la procedura seguente:
    
1. Fare clic sul pulsante di Windows nell'angolo inferiore sinistro dello schermo e scegliere Esegui. Nella casella Apri digitare **regedit**e quindi scegliere OK. 
    
2. Selezionare Sì quando viene richiesto di consentire l'Editor del Registro di sistema per apportare modifiche al dispositivo.
    
3. Nell'Editor del Registro di sistema, aggiungere un valore string di **SharedComputerLicensing** sia impostata su 1 in HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration. 
    
7. Nel server RDS * * *effettuare l'accesso un utente finale* * * e [verificare che l'attivazione di computer condiviso sia abilitato per Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).
    
Per ulteriori informazioni sui prerequisiti, istruzioni di installazione e indicazioni per le installazioni personalizzate utilizzando lo strumento di distribuzione di Office, vedere [Distribuzione di Office 365 ProPlus tramite Servizi Desktop remoto](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).
  
Per correggere gli errori relativi all'attivazione di computer condiviso, vedere [risolvere i problemi con l'attivazione di computer condiviso per Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  

