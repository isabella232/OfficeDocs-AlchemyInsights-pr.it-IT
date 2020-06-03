---
title: I criteri di conservazione nell'interfaccia di amministrazione di Exchange non funzionano
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 3040365b9d686bcbcce60977ee9bdbbaffc70b24
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44502611"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Criteri di conservazione nell'interfaccia di amministrazione di Exchange

 **Problema:** I criteri di conservazione appena creati o aggiornati nell'interfaccia di amministrazione di Exchange non vengono applicati alle cassette postali o gli elementi non vengono spostati nella cassetta postale di archiviazione o sono stati eliminati. 
  
 **Cause principali:**
  
- Questo può essere dovuto al fatto che l' **Assistente cartelle gestite** non ha elaborato la cassetta postale dell'utente. L'Assistente cartelle gestite tenta di elaborare tutte le cassette postali nell'organizzazione basata su cloud una volta ogni sette giorni. Se si modifica un tag di conservazione o si applica un criterio di conservazione diverso a una cassetta postale, è possibile attendere che la cartella gestita contribuisca a elaborare la cassetta postale o che sia possibile eseguire il cmdlet Start-ManagedFolderAssistant per avviare l'Assistente cartelle gestite per elaborare una cassetta postale specifica. L'esecuzione di questo cmdlet è utile per testare o risolvere i problemi relativi a un criterio di conservazione o a un tag di conservazione. Per ulteriori informazioni, vedere [eseguire l'Assistente cartelle gestite](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Soluzione:** Eseguire il seguente comando per avviare l'Assistente cartelle gestite per una cassetta postale specifica:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Questo può verificarsi anche se **RetentionHold** è stato **abilitato** sulla cassetta postale. Se la cassetta postale è stata inserita in una RetentionHold, i criteri di conservazione nella cassetta postale non verranno elaborati in quel periodo. Per ulteriori informazioni sull'impostazione RetentionHold, vedere: [conservazione delle cassette postali](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Soluzione**
    
  - Controllare lo stato dell'impostazione RetentionHold nella cassetta postale specifica in [Exo PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Per **disabilitare** RetentionHold in una cassetta postale specifica, eseguire il comando seguente:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - A questo punto, eseguire di nuovo l'Assistente cartelle gestite:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Nota:** Se una cassetta postale è inferiore a 10 MB, l'Assistente cartelle gestite non elaborerà automaticamente la cassetta postale.
 
Per ulteriori informazioni sui criteri di conservazione nell'interfaccia di amministrazione di Exchange, vedere:
- [Tag di conservazione e criteri di conservazione](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Applicazione dei criteri di conservazione alle cassette postali](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Aggiungere o rimuovere tag di conservazione](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Come identificare il tipo di blocco applicato a una cassetta postale](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
