---
title: Strumento di diagnostica dei servizi per Windows Virtual Desktop
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
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/14/2020
ms.locfileid: "49665825"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Strumento di diagnostica dei servizi per Windows Virtual Desktop

Windows Virtual Desktop (WVD) offre uno strumento di diagnostica che consente agli amministratori di identificare gli errori tramite una singola interfaccia. Questo strumento consente di registrare le informazioni correlate alla diagnostica ogni volta che WVD viene utilizzato da un utente assegnato a un ruolo WVD. Ogni log contiene informazioni sul ruolo WVD coinvolto nell'attività, i messaggi di errore visualizzati durante la sessione e le informazioni sul tenant e sull'utente. L'analisi dei log di Azure può essere configurata per acquisire il log attività creato dallo strumento di diagnostica. Ecco come:

1. Creare un'area di lavoro di analisi dei log con il [portale di Azure](https://go.microsoft.com/fwlink/?linkid=2129500) o [PowerShell di Azure](https://go.microsoft.com/fwlink/?linkid=2129501).
1. [Connettere i computer Windows a Azure monitor](https://go.microsoft.com/fwlink/?linkid=2129913). Ottenere l'ID dell'area di lavoro e la chiave primaria dell'area di lavoro. L'installazione guidata ha bisogno di queste informazioni per configurare correttamente l'agente e per garantire che sia in grado di comunicare con Azure monitor.
1. [Inserire i dati di diagnostica nell'area di lavoro](https://go.microsoft.com/fwlink/?linkid=2128284). È possibile inviare i dati di diagnostica dal tenant di WVD all'analisi dei log per l'area di lavoro.
1. [Identificare e diagnosticare i problemi](https://go.microsoft.com/fwlink/?linkid=2128338) interni o esterni rispetto a Wvd.

Per ulteriori informazioni sulla configurazione dello strumento di diagnostica dei servizi per WVD, vedere [use log Analytics for the Diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2128084).
