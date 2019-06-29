---
title: Utilizzo dello strumento di distribuzione di Office
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: 998f914f38fa9d1925f7003e634d7f11550f47da
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/28/2019
ms.locfileid: "35365529"
---
# <a name="using-the-office-deployment-tool-odt"></a>Utilizzo dello strumento di distribuzione di Office (ODT)

È possibile utilizzare lo strumento di distribuzione di Office per distribuire Office 365 versioni di Office. Lo strumento di distribuzione di Office (Setup. exe) viene eseguito dalla riga di comando e utilizza un file XML di configurazione per determinare le impostazioni da applicare durante la distribuzione di Office.
  
1. Scaricare la versione più recente dello strumento di distribuzione di Office dall' [area download Microsoft](http://go.microsoft.com/fwlink/p/?LinkID=626065).

2. Utilizzare lo [strumento di personalizzazione di Office](https://config.office.com) per selezionare le preferenze di distribuzione e creare il file XML di configurazione. Esportare il file di configurazione e posizionarlo localmente nella stessa cartella in cui si trova Setup. exe.

    **Nota:** I problemi di installazione di Office si verificano generalmente a causa di file di configurazione non configurati o malformatted. Per evitare problemi di questo tipo, è consigliabile utilizzare lo strumento di personalizzazione di Office per creare il file di configurazione. È inoltre possibile importare i file di configurazione esistenti nello strumento di personalizzazione di Office.

3. Da un prompt dei comandi con privilegi elevati, passare al percorso in cui Setup. exe risiede ed eseguire lo strumento di distribuzione di Office in modalità di download e specificare il file di configurazione appena salvato. In questo esempio, il file di configurazione è denominato Configuration. XML:
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. Eseguire lo strumento di distribuzione di Office in modalità configurazione e specificare il file di configurazione.
    
  ```
  setup.exe /configure Configuration.xml
  ```

    **Nota:** È necessario eseguire questo passaggio dal computer client in cui si desidera installare Office ed è necessario disporre delle autorizzazioni di amministratore locale su tale computer.

Per ulteriori informazioni sull'utilizzo dello strumento di distribuzione di Office per gli scenari di distribuzione di Office 365 ProPlus, vedere [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). Per ulteriori informazioni su come utilizzare lo strumento di personalizzazione di Office, vedere [Panoramica dello strumento di personalizzazione di Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
