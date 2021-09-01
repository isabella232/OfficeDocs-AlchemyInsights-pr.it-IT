---
title: Imposizione dei limiti di ricezione delle cassette postali
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/31/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13711"
- "9008580"
ms.openlocfilehash: c1ba5ab10b102680cec52f4e0740c3dd2ceaccbd
ms.sourcegitcommit: a36ec7eda49536933dc8c6f9319cf7320e8aa04d
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/31/2021
ms.locfileid: "58829161"
---
# <a name="mailbox-receiving-limit-enforcement"></a>Imposizione dei limiti di ricezione delle cassette postali

Microsoft ha recentemente iniziato a imporre la soglia per cassetta postale di 3600 messaggi all'ora. Per altre informazioni, vedere [Limiti di Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-limits). Le cassette postali di Microsoft 365 che ricevono più di 3600 messaggi in un'ora vengono limitate per i successivi 60 minuti. 

Viene inoltre applicato il limite delle coppie mittente-destinatario (SRP) che blocca i messaggi ricevuti da una cassetta postale di Microsoft 365 da un mittente specifico. Se un singolo mittente invia oltre il 33% della soglia totale o 1200 messaggi per ogni ora di distribuzione a un destinatario specifico, viene raggiunto il limite SRP e la cassetta postale non accetta più i messaggi da tale mittente. Note:

- Questo limite è applicato ai messaggi di posta elettronica ricevuti da altri tenant, mittenti locali o Internet.
- Il recapito della posta elettronica alla cassetta postale viene bloccato per i successivi 60 minuti. 
- I mittenti di queste cassette postali ricevono un rapporto di mancato recapito (5.2.121 o 5.2.122) che indica che la cassetta postale ha superato la soglia di recapito massima. L'intra-tenant (posta all'interno dello stesso tenant) continua a essere recapitato.
- Quando viene applicato il limite SRP, la cassetta postale di ricezione continua ad accettare i messaggi provenienti da altri mittenti.

Gli amministratori possono monitorare l'attività corrente delle cassette postali accedendo a un nuovo report e informazioni dettagliate nell'interfaccia di amministrazione di Exchange denominata "Cassette postali che superano i limiti di ricezione". Le informazioni dettagliate vengono visualizzate solo se un tenant ha cassette postali non autorizzate, mentre il report viene sempre visualizzato nel dashboard, ma è vuoto a meno che un tenant non abbia cassette postali non autorizzate.

Per ulteriori informazioni sui limiti di ricezione delle informazioni dettagliate, vedere [Informazioni sulle cassette postali che superano i limiti di ricezione nel nuovo EAC.](https://docs.microsoft.com/exchange/monitoring/mail-flow-insights/mailboxes-exceeding-receiving-limits-insights)

Per ulteriori informazioni sul rapporto superamento dei limiti di ricezione, vedere [Informazioni sulle cassette postali che superano i limiti di ricezione nel nuovo EAC.](https://docs.microsoft.com/exchange/monitoring/mail-flow-reports/mailboxes-exceeding-receiving-limits-report)