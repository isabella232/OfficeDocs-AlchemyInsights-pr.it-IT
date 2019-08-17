---
title: I criteri di conservazione nell'interfaccia di amministrazione di Exchange non funzionano
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: d0af4c933f262fe1ec4c2a6ff16d5f6195398b0d
ms.sourcegitcommit: e98443a049108e0dc83d63895af66944bdb1f108
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/16/2019
ms.locfileid: "36444812"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="d4111-102">Criteri di conservazione nell'interfaccia di amministrazione di Exchange</span><span class="sxs-lookup"><span data-stu-id="d4111-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="d4111-103">**Problema:** I criteri di conservazione appena creati o aggiornati nell'interfaccia di amministrazione di Exchange non vengono applicati alle cassette postali o gli elementi non vengono spostati nella cassetta postale di archiviazione o sono stati eliminati.</span><span class="sxs-lookup"><span data-stu-id="d4111-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="d4111-104">**Cause principali:**</span><span class="sxs-lookup"><span data-stu-id="d4111-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="d4111-105">Questo può essere dovuto al fatto che l' **Assistente cartelle gestite** non ha elaborato la cassetta postale dell'utente.</span><span class="sxs-lookup"><span data-stu-id="d4111-105">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="d4111-106">L'Assistente cartelle gestite tenta di elaborare tutte le cassette postali nell'organizzazione basata su cloud una volta ogni sette giorni.</span><span class="sxs-lookup"><span data-stu-id="d4111-106">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="d4111-107">Se si modifica un tag di conservazione o si applica un criterio di conservazione diverso a una cassetta postale, è possibile attendere che la cartella gestita contribuisca a elaborare la cassetta postale o che sia possibile eseguire il cmdlet Start-ManagedFolderAssistant per avviare l'Assistente cartelle gestite per elaborare una specifica cassetta postale.</span><span class="sxs-lookup"><span data-stu-id="d4111-107">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="d4111-108">L'esecuzione di questo cmdlet è utile per testare o risolvere i problemi relativi a un criterio di conservazione o a un tag di conservazione.</span><span class="sxs-lookup"><span data-stu-id="d4111-108">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="d4111-109">Per ulteriori informazioni, vedere [eseguire l'Assistente cartelle gestite](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="d4111-109">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="d4111-110">**Soluzione:** Eseguire il seguente comando per avviare l'Assistente cartelle gestite per una cassetta postale specifica:</span><span class="sxs-lookup"><span data-stu-id="d4111-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="d4111-111">Questo può verificarsi anche se **RetentionHold** è stato **abilitato** sulla cassetta postale.</span><span class="sxs-lookup"><span data-stu-id="d4111-111">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="d4111-112">Se la cassetta postale è stata inserita in una RetentionHold, i criteri di conservazione nella cassetta postale non verranno elaborati in quel periodo.</span><span class="sxs-lookup"><span data-stu-id="d4111-112">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="d4111-113">Per ulteriori informazioni sull'impostazione RetentionHold, vedere: [conservazione delle cassette postali](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="d4111-113">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="d4111-114">**Soluzione**</span><span class="sxs-lookup"><span data-stu-id="d4111-114">**Solution:**</span></span>
    
  - <span data-ttu-id="d4111-115">Controllare lo stato dell'impostazione RetentionHold nella cassetta postale specifica in [Exo PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="d4111-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="d4111-116">Per **disabilitare** RetentionHold in una cassetta postale specifica, eseguire il comando seguente:</span><span class="sxs-lookup"><span data-stu-id="d4111-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="d4111-117">A questo punto, eseguire di nuovo l'Assistente cartelle gestite:</span><span class="sxs-lookup"><span data-stu-id="d4111-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="d4111-118">**Nota:** Se una cassetta postale è inferiore a 10 MB, l'Assistente cartelle gestite non elaborerà automaticamente la cassetta postale.</span><span class="sxs-lookup"><span data-stu-id="d4111-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="d4111-119">Per ulteriori informazioni sui criteri di conservazione nell'interfaccia di amministrazione di Exchange, vedere:</span><span class="sxs-lookup"><span data-stu-id="d4111-119">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="d4111-120">Tag di conservazione e criteri di conservazione</span><span class="sxs-lookup"><span data-stu-id="d4111-120">Retention tags and retention policies</span></span>](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="d4111-121">Applicazione dei criteri di conservazione alle cassette postali</span><span class="sxs-lookup"><span data-stu-id="d4111-121">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="d4111-122">Aggiungere o rimuovere tag di conservazione</span><span class="sxs-lookup"><span data-stu-id="d4111-122">Add or remove retention tags</span></span>](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="d4111-123">Come identificare il tipo di blocco posizionato su una cassetta postale</span><span class="sxs-lookup"><span data-stu-id="d4111-123">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/en-us/office365/securitycompliance/identify-a-hold-on-an-exchange-online-mailbox)
