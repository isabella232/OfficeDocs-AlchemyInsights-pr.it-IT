---
title: File su richiesta
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6432"
- "9003530"
ms.openlocfilehash: 846cda97ccd52fcb43ae4a44f73deeaaa6dc093d
ms.sourcegitcommit: b7bbe4c5419668ce8e84196db382032ca09cd176
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/08/2020
ms.locfileid: "47406582"
---
# <a name="configure-files-on-demand"></a>Configurare File su richiesta

La funzionalità File di OneDrive su richiesta consente di accedere a tutti i file di OneDrive senza doverli scaricare tutti occupando spazio di archiviazione nel dispositivo.

Per configurare File su richiesta nel PC:

1. Selezionare l'icona della nuvola bianca o blu di **OneDrive** nell'area di notifica della barra delle applicazioni di Windows. Selezionare l'icona dell'ingranaggio di **Guida e impostazioni** e quindi **Impostazioni**.
2. Nella scheda **Impostazioni** selezionare la casella **Risparmia spazio e scarica i file quando li usi**.  

È anche possibile configurare File su richiesta con il registro di sistema.

Se si disabilita questa impostazione, gli utenti di Windows 10 ricevono lo stesso comportamento di sincronizzazione degli utenti delle versioni precedenti di Windows e non sono in grado di attivare File su richiesta. Se non si configura l'impostazione, gli utenti possono attivare o disattivare File su richiesta a piacimento.

L'abilitazione di questo criterio imposta il valore della chiave del Registro di sistema seguente su 1. La disabilitazione di questo criterio imposta il valore della seguente chiave del registro di sistema su 0.

`[HKLM\SOFTWARE\Policies\Microsoft\OneDrive]"FilesOnDemandEnabled"="dword:00000001"`

Se l'opzione File su richiesta non è visualizzata nelle Impostazioni, verificare che il tipo di avvio del servizio "Driver filtro dei file di Windows Cloud" sia impostato su 2 (AUTO_START). L'abilitazione di questo criterio imposta il valore della seguente chiave del registro di sistema su 2.

`[HKLM\SYSTEM\CurrentControlSet\Services\CldFlt]"Start"="dword:00000002"`