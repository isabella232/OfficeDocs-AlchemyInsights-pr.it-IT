---
title: Criteri di conservazione nell'interfaccia di amministrazione di Exchange non funziona
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 0ceb1737040f0304bfe8b611241ce1deef487652
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/24/2019
ms.locfileid: "29476153"
---
 **Problema:** Appena creato o i criteri di conservazione aggiornati nell'interfaccia di amministrazione di Exchange non si applicano alle cassette postali o gli elementi non vengono spostati la cassetta postale di archiviazione o eliminati. 
  
 **Cause principali:**
  
- È possibile che **l'Assistente cartelle gestite** non elaborato cassetta postale dell'utente. L'Assistente cartelle gestite tenta di elaborare tutte le cassette postali nell'organizzazione basata su cloud ogni sette giorni. Se si modifica un tag di conservazione o applicare un criterio di conservazione diversi a una cassetta postale, è possibile attendere fino a quando la cartella gestita assistere elaborata la cassetta postale o è possibile eseguire il cmdlet Start-ManagedFolderAssistant per avviare l'Assistente cartelle gestite per la stampa in un oggetto specifico cassetta postale. Esecuzione di questo cmdlet è utile per i test o la risoluzione dei problemi di un criterio di conservazione o le impostazioni di tag di conservazione. Per ulteriori informazioni, visitare il sito [eseguito l'Assistente cartelle gestite](https://msdn.microsoft.com/en-us/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Soluzione:** Eseguire il comando seguente per avviare l'Assistente cartelle gestite per una cassetta postale specifica: 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Ciò può inoltre verificarsi se **RetentionHold** è stato **abilitato** per la cassetta postale. Se la cassetta postale sia stata inserita in un RetentionHold, il criterio di conservazione della cassetta postale non verrà elaborato periodo di tempo. Per ulteriori informazioni relative sui, vedere Impostazione RetentionHold: [Mantenimento delle cassette postali](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Soluzione**
    
  - Verificare lo stato dell'impostazione RetentionHold nella cassetta postale specifica [EXO](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)PowerShell:
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Eseguire il seguente comando per **disabilitare** RetentionHold in una cassetta postale specifica: 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - A questo punto, eseguire nuovamente la cartella gestita Assistente:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Nota:** Se una cassetta postale è inferiore a 10 MB, l'Assistente cartelle gestite non elaborerà automaticamente alla cassetta postale. 
  

