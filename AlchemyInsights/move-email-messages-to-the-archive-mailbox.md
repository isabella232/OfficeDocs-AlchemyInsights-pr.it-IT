---
title: Spostamento dei messaggi di posta elettronica alla cassetta postale di archiviazione
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 41d6825b568263fb7b09066b65235aa348415bae
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/15/2019
ms.locfileid: "28296915"
---
Problemi durante l'archiviazione di elementi per la cassetta postale di archivio. Verificare che siano state eseguite le operazioni seguenti:
  
1. Verificare che sia stato abilitato un **archivio delle cassette postali** . In caso contrario, utilizzare i passaggi in [questo articolo](https://docs.microsoft.com/en-us/office365/securitycompliance/enable-archive-mailboxes) per abilitare la cassetta postale di archivio. 
    
2. Nell'interfaccia di amministrazione di Exchange, selezionare **I tag di conservazione** in **Gestione della conformità**, creare un **tag di conservazione** con l'azione **Sposta nell'archivio** che contiene il **Periodo di conservazione**di desiderato.
    
3. Nell'interfaccia di amministrazione di Exchange, selezionare **I criteri di conservazione**, creare un **Criterio di conservazione** e aggiungere i tag di conservazione **Sposta nell'archivio** per quel criterio. 
    
4. [Assegnare il criterio di conservazione](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) cassetta postale dell'utente specifico. Lo stesso criterio verrà applicato a **principale** e cassetta postale di **archivio** . 
    
Cassetta postale dell'utente deve avere un criterio di archiviazione per spostare gli elementi di cassetta postale di archiviazione. Potrebbe essere necessario forzare il gestiti cartella Assistente (MFA) per l'esecuzione e applicare nuove impostazioni cassetta postale dell'utente. Eseguire il comando seguente durante la [connessione a PowerShell EXO](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) per avviare l'Assistente cartelle gestite per una cassetta postale specifica: 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

Ottenere ulteriori informazioni sull'impostazione di criteri di archiviazione, vedere [impostazione di un criterio di archiviazione e l'eliminazione delle cassette postali](https://docs.microsoft.com/en-us/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  

