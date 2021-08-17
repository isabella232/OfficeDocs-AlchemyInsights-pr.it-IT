---
title: Utilizzo dello strumento Office distribuzione
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
ms.openlocfilehash: 39a011d4b121492d222ff620e70d9860231b7bcfe0d7fd2ecfd93de1ef502f5f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083774"
---
# <a name="using-the-office-deployment-tool-odt"></a>Uso dello Office Deployment Tool (ODT)

Puoi usare lo Office Deployment Tool (ODT) per distribuire Office 365 versioni di Office. Lo Office Deployment Tool (setup.exe) viene eseguito dalla riga di comando e utilizza un file XML di configurazione per determinare le impostazioni da applicare durante la distribuzione di Office.
  
1. Scaricare la versione più recente dello strumento Office distribuzione [dall'Area download Microsoft.](https://go.microsoft.com/fwlink/p/?LinkID=626065)

2. Utilizzare lo [Strumento Office per selezionare](https://config.office.com) le preferenze di distribuzione e creare il file XML di configurazione. Esportare il file di configurazione e posizionarlo localmente nella stessa cartella in cui si trova setup.exe file.

    **Nota: Office** problemi di installazione si verificano in genere a causa di file di configurazione non configurati correttamente o non formattati correttamente. Per evitare tali problemi, è consigliabile utilizzare lo Strumento di personalizzazione Office per creare il file di configurazione. È inoltre possibile importare file di configurazione esistenti nello Office Customization Tool.

3. Da un prompt dei comandi con privilegi elevati passare al percorso in cui risiede setup.exe ed eseguire lo strumento di distribuzione di Office in modalità download e specificare il file di configurazione appena salvato. In questo esempio, il file di configurazione è denominato Configuration.xml:

```setup.exe /download Configuration.xml```

4.Eseguire lo strumento Office distribuzione in modalità di configurazione e specificare il file di configurazione.

```setup.exe /configure Configuration.xml```

**Nota:** È necessario eseguire questo passaggio dal computer client in cui si desidera installare Office e disporre delle autorizzazioni di amministratore locale per tale computer.

Per ulteriori informazioni sull'Office di distribuzione per gli scenari di Microsoft 365 Apps for enterprise, vedere [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool). Per ulteriori informazioni su come utilizzare lo strumento di personalizzazione Office, vedere [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
