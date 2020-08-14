---
title: Cambiare i canali di aggiornamento per le app di Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1740"
- "9000140"
ms.openlocfilehash: fb69bce40ab56b162c715af6a0647c8219c5564f
ms.sourcegitcommit: dab885f2cb99057e959fb9be334f5a3a26a64058
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/13/2020
ms.locfileid: "46665466"
---
# <a name="change-update-channels-for-office-apps"></a>Cambiare i canali di aggiornamento per le app di Office

Per le nuove installazioni di Office, usare le impostazioni di download del software Office per selezionare il canale di aggiornamento desiderato, quindi installare o reinstallare le app di Office. Per altre informazioni, si veda [Gestire le impostazioni di download del software in Office 365](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365). 

**Nota** Il canale di aggiornamento selezionato con le impostazioni di download del software Office si applica a tutti gli utenti che eseguono nuove installazioni usando il portale di Office 365. Per altre informazioni, si veda [Scaricare e installare o reinstallare Microsoft 365 o Office 2019 in un PC o Mac](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658).   

Per le installazioni di Office esistenti, usare lo strumento di distribuzione di Office (ODT) per passare a un altro canale di aggiornamento:  

1. Scaricare la versione più recente dello strumento di distribuzione di Office (setup.exe) dall'[Area download Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).
2. Identificare il nome del canale a cui si vuole passare. Per altre informazioni, vedere [Opzioni di configurazione per lo strumento di distribuzione di Office](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element).
3. Creare un file XML di configurazione specificando il nome del canale appropriato, ad esempio update.xml.  
    `<Configuration> 
    <Updates **Channel="Monthly"** />  
    </Configuration>`
4. Da un prompt dei comandi con privilegi elevati, passare alla posizione della cartella in cui risiede il file setup.exe ed eseguire il comando seguente:  
    a. setup.exe /configura update.xml
5. Avviare un'applicazione di Office, ad esempio Excel, quindi selezionare **File** > **Account**. Nella sezione Informazioni sul prodotto selezionare **Opzioni di aggiornamento** > **Aggiorna ora**.

Per altre informazioni, si veda [Come cambiare canale di aggiornamento per le app di Office esistenti](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel). 

Per cambiare canale di aggiornamento per un gruppo selezionato di utenti o con Configuration Manager (SCCM), configurare l'impostazione del canale di aggiornamento tramite oggetto Criteri di gruppo. Per altre informazioni, vedere [Panoramica dei canali di aggiornamento per Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy). Per informazioni dettagliate, vedere [Come gestire i canali di Office 365 ProPlus per i professionisti IT](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813) e [Gestire gli aggiornamenti alle app di Microsoft 365 con Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager).