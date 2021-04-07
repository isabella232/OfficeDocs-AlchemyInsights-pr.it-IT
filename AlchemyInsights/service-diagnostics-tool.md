---
title: Strumento di diagnostica dei servizi per il Desktop virtuale Windows
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: dfa59c86508c8658c880f4f3f21a002524e909d1
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/05/2021
ms.locfileid: "51590301"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Strumento di diagnostica dei servizi per il Desktop virtuale Windows

Il Desktop virtuale Windows (WVD) offre uno strumento di diagnostica che consente agli amministratori di identificare gli errori tramite un'unica interfaccia. Questo strumento registra le informazioni correlate alla diagnostica ogni volta che viene usato il WVD da un utente a cui è assegnato un ruolo WVD. Ogni log contiene informazioni sul ruolo WVD coinvolto nell'attività, i messaggi di errore visualizzati durante la sessione e le informazioni sul tenant e l'utente. Azure Log Analytics può essere configurato per acquisire il log attività creato dallo strumento di diagnostica tramite questa procedura:

1. Creare un'area di lavoro Log Analytics tramite il [portale di Azure](https://go.microsoft.com/fwlink/?linkid=2129500) o [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).

1. [Connettere i computer Windows al Monitoraggio di Azure](https://go.microsoft.com/fwlink/?linkid=2129913). Ottenere l'ID dell'area di lavoro e la chiave primaria dell'area di lavoro. La configurazione della procedura guidata necessita di queste informazioni per configurare correttamente l'agente e assicurarsi che possa comunicare con il Monitoraggio di Azure.

1. [Eseguire il push dei dati di diagnostica nell'area di lavoro](https://go.microsoft.com/fwlink/?linkid=2128284). È possibile effettuare il push dei dati di diagnostica dal tenant WVD al Log Analytics per l’area di lavoro.

1. [Identificare ed eseguire la diagnostica](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) dei problemi interni o esterni in relazione al Desktop virtuale Windows.

Per altre informazioni sulla configurazione dello strumento di diagnostica del servizio per WVD, vedere Uso di Log Analytics per la funzionalità di diagnostica.