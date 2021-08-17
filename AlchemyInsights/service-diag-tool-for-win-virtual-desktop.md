---
title: Strumento di diagnostica dei servizi per Desktop virtuale Windows
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: 58688e3216ba6777b1a4f76095bd39c81a2d2a8294e06b6bc61c7134f6d589f9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052390"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Strumento di diagnostica dei servizi per Desktop virtuale Windows

Desktop virtuale Windows offre agli amministratori uno strumento di diagnostica per identificare gli errori tramite un'unica interfaccia. Questo strumento registra le informazioni correlate alla diagnostica ogni volta che viene usato Desktop virtuale Windows da un utente a cui è assegnato un ruolo di Desktop virtuale Windows. Ogni log contiene informazioni sul ruolo Desktop virtuale Windows coinvolto nell'attività, i messaggi di errore visualizzati durante la sessione e le informazioni sul tenant e l'utente. Azure Log Analytics può essere configurato per acquisire il log attività creato dallo strumento di diagnostica. Ecco come:

1. Creare un'area di lavoro Log Analytics tramite il [portale di Azure](https://go.microsoft.com/fwlink/?linkid=2129500) o [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).
1. [Connettere i computer Windows al Monitoraggio di Azure](https://go.microsoft.com/fwlink/?linkid=2129913). Ottenere l'ID dell'area di lavoro e la chiave primaria dell'area di lavoro. La configurazione della procedura guidata necessita di queste informazioni per configurare correttamente l'agente e assicurarsi che possa comunicare con il Monitoraggio di Azure.
1. [Eseguire il push dei dati di diagnostica nell'area di lavoro](https://go.microsoft.com/fwlink/?linkid=2128284). È possibile effettuare il push dei dati di diagnostica dal tenant WVD al Log Analytics per l’area di lavoro.
1. [Identificare e diagnosticare i](https://go.microsoft.com/fwlink/?linkid=2128338) problemi interni o esterni in relazione a WVD.

Per altre informazioni sulla configurazione dello strumento di diagnostica del servizio per WVD, vedi [Usare Log Analytics per la funzionalità di diagnostica.](https://go.microsoft.com/fwlink/?linkid=2128084)
