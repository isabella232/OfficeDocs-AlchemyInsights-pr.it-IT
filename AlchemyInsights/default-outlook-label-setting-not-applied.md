---
title: Impostazione Outlook predefinita dell'etichetta non applicata
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000181"
- "13259"
ms.openlocfilehash: 84284554151586ff0a22f983d9494f59b4675f92
ms.sourcegitcommit: 4b92c2648ddba3ad3bc61a22771c59ed5fc76303
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/17/2021
ms.locfileid: "58370212"
---
# <a name="default-outlook-label-setting-not-applied"></a>Impostazione Outlook predefinita dell'etichetta non applicata

Se le impostazioni predefinite dell'etichetta Outlook non vengono applicate correttamente e viene applicata un'etichetta diversa o nessuna etichetta, potrebbe verificarsi un problema noto (MC277818) ed eseguire una delle due opzioni seguenti per risolvere il problema:

**Opzione 1:**

1. Passare a Microsoft 365 Centro conformità > **Soluzioni**  >  **Information Protection**.
1. Selezionare **Criteri etichetta** e selezionare il criterio di etichetta da modificare ( l'impostazione **outlookDefaultlabel** non è impostata correttamente nel criterio etichetta in questione. Eseguire **Get-labelpolicy** per visualizzare questa impostazione, quindi selezionare **Modifica criterio.**
1. Selezionare **Avanti** finché non viene visualizzata l'impostazione Applica questa etichetta predefinita ai messaggi di posta elettronica **,**  disponibile se si seleziona Richiedi agli utenti di applicare un'etichetta **ai** messaggi di posta elettronica e ai documenti dell'erede nella finestra di dialogo Impostazioni criteri.
1. Nella finestra **di dialogo Applica un'etichetta predefinita ai** documenti scegliere Nessuna **nell'elenco** a discesa.
1. Seleziona **Avanti e** Invia **per** salvare le impostazioni dell'etichetta.

**Opzione 2:**

In [Powershell centro](https://docs.microsoft.com/powershell/exchange/connect-to-scc-powershell?view=exchange-ps)sicurezza e conformità, utilizzare il commandlet Set-LabelPolicy per modificare **outlookDefaultlabel** su **None** in {OutlookDefaultLabel="None"}.

Correre: `Set-LabelPolicy -Identity [policy] -AdvancedSettings @{OutlookDefaultLabel="None"}`

Per ulteriori informazioni sulle etichette predefinite per Outlook, vedere [Set a different default label for Outlook](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide-customizations#set-a-different-default-label-for-outlook).