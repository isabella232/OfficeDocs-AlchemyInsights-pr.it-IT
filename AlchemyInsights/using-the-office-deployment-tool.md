---
title: Utilizzo dello strumento di distribuzione di Office
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: f3a5dbfc6b64ccd4f0b19a5f86236336e78838d4
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/17/2020
ms.locfileid: "49085836"
---
# <a name="using-the-office-deployment-tool-odt"></a>Utilizzo dello strumento di distribuzione di Office (ODT)

È possibile utilizzare lo strumento di distribuzione di Office per distribuire Office 365 versioni di Office. Lo strumento di distribuzione di Office (setupodt.exe) viene eseguito dalla riga di comando e utilizza un file XML di configurazione per determinare le impostazioni da applicare durante la distribuzione di Office.
  
1. Scaricare la versione più recente dello strumento di distribuzione di Office dall' [area download Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).

2. Utilizzare lo [strumento di personalizzazione di Office](https://config.office.com) per selezionare le preferenze di distribuzione e creare il file XML di configurazione. Esportare il file di configurazione e posizionarlo localmente nella stessa cartella in cui risiede il setupodt.exe.

    **Nota:** I problemi di installazione di Office si verificano generalmente a causa di file di configurazione non configurati o malformatted. Per evitare problemi di questo tipo, è consigliabile utilizzare lo strumento di personalizzazione di Office per creare il file di configurazione. È inoltre possibile importare i file di configurazione esistenti nello strumento di personalizzazione di Office.

3. Da un prompt dei comandi con privilegi elevati, passare al percorso in cui setupodt.exe risiede ed eseguire lo strumento di distribuzione di Office in modalità download e specificare il file di configurazione appena salvato. In questo esempio, il file di configurazione è denominato Configuration.xml:

```setupodt.exe /download Configuration.xml```

4. eseguire lo strumento di distribuzione di Office in modalità configurazione e specificare il file di configurazione.

```setupodt.exe /configure Configuration.xml```

**Nota:** È necessario eseguire questo passaggio dal computer client in cui si desidera installare Office ed è necessario disporre delle autorizzazioni di amministratore locale su tale computer.

Per ulteriori informazioni sull'utilizzo dello strumento di distribuzione di Office per gli scenari di distribuzione di Microsoft 365 Apps for Enterprise, vedere [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool). Per ulteriori informazioni su come utilizzare lo strumento di personalizzazione di Office, vedere [Panoramica dello strumento di personalizzazione di Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
