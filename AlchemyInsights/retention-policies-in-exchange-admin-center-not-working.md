---
title: I criteri di conservazione nell'interfaccia di amministrazione di Exchange non funzionano
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 1fee2361b2dd6e0989d430a17aebb13bd5948578
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740514"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Criteri di conservazione nell'interfaccia di amministrazione di Exchange

Se si desidera che vengano eseguiti controlli automatici per le impostazioni indicate di seguito, selezionare il pulsante indietro <--nella parte superiore di questa pagina e quindi immettere l'indirizzo di posta elettronica dell'utente che ha problemi con i criteri di conservazione.

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
