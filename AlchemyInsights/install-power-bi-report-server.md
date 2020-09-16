---
title: Installare il server di report di Power BI
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1304"
- "2500001"
ms.openlocfilehash: 3ea596547093773ab872ca34e8dd3a4e49e59fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47755099"
---
# <a name="install-power-bi-report-server"></a>Installare il server di report di Power BI

1. Individuare il percorso del PowerBIReportServer.exe e avviare il programma di installazione.

2. Selezionare **Install Power bi report server**.

3. Scegliere un'edizione da installare e quindi fare clic su **Avanti**.

4. È possibile scegliere Evaluation o Developer Edition dal menu a discesa.  In caso contrario, è possibile immettere un codice "Product Key" per il server acquisito dal servizio Power BI o dal centro servizi per contratti multilicenza. Per ulteriori informazioni su come ottenere il codice Product Key, vedere la sezione prima di iniziare. Leggere e accettare le condizioni di licenza e quindi fare clic su **Avanti**.

5. È necessario disporre di un modulo di gestione di database per archiviare il database del server di report. Fare clic su **Avanti** per installare solo il server di report.

6. Specificare il percorso di installazione per il server di report. Selezionare **Installa** per continuare.

7. Dopo aver completato l'installazione, selezionare **Configura server di report** per avviare Gestione configurazione Reporting Services.

Non è necessario un server del motore di database di SQL Server disponibile al momento dell'installazione. Sarà necessario eseguire una configurazione di Reporting Services dopo l'installazione.

Per ulteriori informazioni: https://docs.microsoft.com/power-bi/report-server/install-report-server
