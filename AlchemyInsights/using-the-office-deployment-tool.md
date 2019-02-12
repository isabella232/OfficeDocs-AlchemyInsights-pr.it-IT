---
title: Utilizzo dello strumento di distribuzione di Office
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: c7e0e96f225030590fdd516eaf3115c93a6335b6
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29898650"
---
# <a name="using-the-office-deployment-tool-odt"></a>Using the Office Deployment Tool (ODT)

Utilizzare Office Deployment Tool (ODT) per distribuire Office 365 le versioni di Office. Lo strumento di distribuzione di Office (setup.exe) eseguire dalla riga di comando e viene utilizzato un file XML di configurazione per determinare le impostazioni da applicare durante la distribuzione di Office.
  
1. Scaricare la versione più recente di Office Deployment Tool dall' [Area Download Microsoft](http://go.microsoft.com/fwlink/p/?LinkID=626065).
    
2. Utilizzare [Office Customization Tool (OCT)](https://config.office.com) per selezionare le preferenze di distribuzione e creare file di configurazione XML. Esportare il file di configurazione e inserirli localmente nella stessa cartella in cui risiede il setup.exe. 
    
    **Nota:** Installazione di Office in genere si verificano problemi dovuti a non correttamente configurato o i file di configurazione valido. Per evitare tali problemi, è consigliabile utilizzare lo strumento di personalizzazione di Office per creare il file di configurazione. È inoltre possibile importare file di configurazione esistenti nello strumento di personalizzazione di Office. 
    
3. Da un prompt dei comandi con privilegi elevati, passare alla posizione in cui risiede setup.exe eseguire lo strumento di distribuzione di Office in modalità download e specificare il file di configurazione che appena salvato. In questo esempio il file di configurazione denominato Configuration. XML:
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. Eseguire lo strumento di distribuzione di Office in modalità configure e specificare il file di configurazione.
    
  ```
  setup.exe /configure Configuration.xml
  ```

    **Nota:** È necessario eseguire questo passaggio dal computer client in cui si desidera installare Office, quindi è necessario disporre delle autorizzazioni di amministratore locale nel computer. 
    
Per ulteriori informazioni sull'utilizzo dello strumento di distribuzione di Office per gli scenari di distribuzione di Office 365 ProPlus, vedere [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). Per ulteriori informazioni su come utilizzare lo strumento di personalizzazione di Office, vedere [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
  

