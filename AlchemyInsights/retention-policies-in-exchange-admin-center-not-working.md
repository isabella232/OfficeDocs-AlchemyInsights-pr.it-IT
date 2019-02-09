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
ms.openlocfilehash: 73e8db432afccb73b872ec7a3ce84c25f1ba7f25
ms.sourcegitcommit: ca06ef831226d629de3057a0df85e017b80f3356
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 02/08/2019
ms.locfileid: "29786774"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="a3bac-102">Criteri di conservazione nell'interfaccia di amministrazione di Exchange</span><span class="sxs-lookup"><span data-stu-id="a3bac-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="a3bac-103">**Problema:** Appena creato o i criteri di conservazione aggiornati nell'interfaccia di amministrazione di Exchange non si applicano alle cassette postali o gli elementi non vengono spostati la cassetta postale di archiviazione o eliminati.</span><span class="sxs-lookup"><span data-stu-id="a3bac-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="a3bac-104">**Cause principali:**</span><span class="sxs-lookup"><span data-stu-id="a3bac-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="a3bac-p101">È possibile che **l'Assistente cartelle gestite** non elaborato cassetta postale dell'utente. L'Assistente cartelle gestite tenta di elaborare tutte le cassette postali nell'organizzazione basata su cloud ogni sette giorni. Se si modifica un tag di conservazione o applicare un criterio di conservazione diversi a una cassetta postale, è possibile attendere fino a quando la cartella gestita assistere elaborata la cassetta postale o è possibile eseguire il cmdlet Start-ManagedFolderAssistant per avviare l'Assistente cartelle gestite per la stampa in un oggetto specifico cassetta postale. Esecuzione di questo cmdlet è utile per i test o la risoluzione dei problemi di un criterio di conservazione o le impostazioni di tag di conservazione. Per ulteriori informazioni, visitare il sito [eseguito l'Assistente cartelle gestite](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="a3bac-p101">This may be because the **Managed Folder Assistant** has not processed the user's mailbox. The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days. If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox. Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings. For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="a3bac-110">**Soluzione:** Eseguire il comando seguente per avviare l'Assistente cartelle gestite per una cassetta postale specifica:</span><span class="sxs-lookup"><span data-stu-id="a3bac-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span> 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="a3bac-p102">Ciò può inoltre verificarsi se **RetentionHold** è stato **abilitato** per la cassetta postale. Se la cassetta postale sia stata inserita in un RetentionHold, il criterio di conservazione della cassetta postale non verrà elaborato periodo di tempo. Per ulteriori informazioni relative sui, vedere Impostazione RetentionHold: [Mantenimento delle cassette postali](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="a3bac-p102">This may also be occur if **RetentionHold** has been **enabled** on the mailbox. If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time. For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="a3bac-114">**Soluzione:**</span><span class="sxs-lookup"><span data-stu-id="a3bac-114">**Solution:**</span></span>
    
  - <span data-ttu-id="a3bac-115">Verificare lo stato dell'impostazione RetentionHold nella cassetta postale specifica [EXO](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)PowerShell:</span><span class="sxs-lookup"><span data-stu-id="a3bac-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="a3bac-116">Eseguire il seguente comando per **disabilitare** RetentionHold in una cassetta postale specifica:</span><span class="sxs-lookup"><span data-stu-id="a3bac-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span> 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="a3bac-117">A questo punto, eseguire nuovamente la cartella gestita Assistente:</span><span class="sxs-lookup"><span data-stu-id="a3bac-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="a3bac-118">**Nota:** Se una cassetta postale è inferiore a 10 MB, l'Assistente cartelle gestite non elaborerà automaticamente alla cassetta postale.</span><span class="sxs-lookup"><span data-stu-id="a3bac-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span> 
  

