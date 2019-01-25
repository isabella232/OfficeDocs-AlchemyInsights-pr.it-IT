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
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/24/2019
ms.locfileid: "29475899"
---
<span data-ttu-id="56ffc-p101">Problemi durante l'archiviazione di elementi per la cassetta postale di archivio. Verificare che siano state eseguite le operazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="56ffc-p101">Having problems archiving items to the Archive mailbox. Make sure you have performed the following steps:</span></span>
  
1. <span data-ttu-id="56ffc-p102">Verificare che sia stato abilitato un **archivio delle cassette postali** . In caso contrario, utilizzare i passaggi in [questo articolo](https://docs.microsoft.com/en-us/office365/securitycompliance/enable-archive-mailboxes) per abilitare la cassetta postale di archivio.</span><span class="sxs-lookup"><span data-stu-id="56ffc-p102">Confirm that an **Archive mailbox** has been enabled. If not, use steps in [this article](https://docs.microsoft.com/en-us/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span> 
    
2. <span data-ttu-id="56ffc-106">Nell'interfaccia di amministrazione di Exchange, selezionare **I tag di conservazione** in **Gestione della conformità**, creare un **tag di conservazione** con l'azione **Sposta nell'archivio** che contiene il **Periodo di conservazione**di desiderato.</span><span class="sxs-lookup"><span data-stu-id="56ffc-106">In the Exchange Admin Center, select **Retention Tags** under **Compliance Management**, create a **Retention tag** with the **Move to Archive** action containing the desired **Retention Age**.</span></span>
    
3. <span data-ttu-id="56ffc-107">Nell'interfaccia di amministrazione di Exchange, selezionare **I criteri di conservazione**, creare un **Criterio di conservazione** e aggiungere i tag di conservazione **Sposta nell'archivio** per quel criterio.</span><span class="sxs-lookup"><span data-stu-id="56ffc-107">In the Exchange Admin Center, select **Retention Policies**, create a **Retention Policy** and add your **Move to Archive** retention tag to that policy.</span></span> 
    
4. <span data-ttu-id="56ffc-p103">[Assegnare il criterio di conservazione](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) cassetta postale dell'utente specifico. Lo stesso criterio verrà applicato a **principale** e cassetta postale di **archivio** .</span><span class="sxs-lookup"><span data-stu-id="56ffc-p103">[Assign the Retention Policy](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox. The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span> 
    
<span data-ttu-id="56ffc-p104">Cassetta postale dell'utente deve avere un criterio di archiviazione per spostare gli elementi di cassetta postale di archiviazione. Potrebbe essere necessario forzare il gestiti cartella Assistente (MFA) per l'esecuzione e applicare nuove impostazioni cassetta postale dell'utente. Eseguire il comando seguente durante la [connessione a PowerShell EXO](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) per avviare l'Assistente cartelle gestite per una cassetta postale specifica:</span><span class="sxs-lookup"><span data-stu-id="56ffc-p104">The user's mailbox should now have an Archive policy to move items to the Archive mailbox. It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox. Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span> 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

<span data-ttu-id="56ffc-113">Ottenere ulteriori informazioni sull'impostazione di criteri di archiviazione, vedere [impostazione di un criterio di archiviazione e l'eliminazione delle cassette postali](https://docs.microsoft.com/en-us/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="56ffc-113">Want more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/en-us/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  

