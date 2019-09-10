---
title: Spostare i messaggi di posta elettronica nella cassetta postale di archiviazione
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 5592bc7d4566e3498c33bbf9488db7f46ec58842
ms.sourcegitcommit: 8864b5789d9905916039081b53530c7e6d8bc529
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822166"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="7a4a2-102">Spostare la posta elettronica nella cassetta postale di archiviazione</span><span class="sxs-lookup"><span data-stu-id="7a4a2-102">Move email to the archive mailbox</span></span>

1. <span data-ttu-id="7a4a2-103">Verificare che sia stata abilitata una **cassetta postale di archiviazione** .</span><span class="sxs-lookup"><span data-stu-id="7a4a2-103">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="7a4a2-104">In caso contrario, utilizzare la procedura descritta in [questo articolo](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) per abilitare la cassetta postale di archiviazione.</span><span class="sxs-lookup"><span data-stu-id="7a4a2-104">If not, use the steps in [this article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="7a4a2-105">Per archiviare automaticamente i messaggi nella cassetta postale di archiviazione, è necessario impostare un tag di conservazione con l'azione **Sposta nell'archivio** su **applicato automaticamente all'intero tag della cassetta postale (impostazione predefinita)**.</span><span class="sxs-lookup"><span data-stu-id="7a4a2-105">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="7a4a2-106">Utilizzare la procedura seguente per creare il tag: [archivio predefinito](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag)tag.</span><span class="sxs-lookup"><span data-stu-id="7a4a2-106">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="7a4a2-107">Successivamente, aggiungere il tag di **archiviazione** al criterio di conservazione.</span><span class="sxs-lookup"><span data-stu-id="7a4a2-107">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="7a4a2-108">Nell'interfaccia di amministrazione di Exchange, scegliere **criteri di conservazione** > aggiungere il **tag Move to Archive** al criterio > **Save**.</span><span class="sxs-lookup"><span data-stu-id="7a4a2-108">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="7a4a2-109">A questo punto, [assegnare il criterio di conservazione](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) alla cassetta postale dell'utente specifico.</span><span class="sxs-lookup"><span data-stu-id="7a4a2-109">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="7a4a2-110">Lo stesso criterio verrà applicato sia alla cassetta postale **principale** che a quella di **archiviazione** .</span><span class="sxs-lookup"><span data-stu-id="7a4a2-110">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="7a4a2-111">Potrebbe essere necessario forzare l'esecuzione dell'Assistente cartelle gestite e applicare le nuove impostazioni alla cassetta postale dell'utente.</span><span class="sxs-lookup"><span data-stu-id="7a4a2-111">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="7a4a2-112">Eseguire il seguente comando quando [si è connessi a Exo PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) per avviare l'Assistente cartelle gestite per una cassetta postale specifica:</span><span class="sxs-lookup"><span data-stu-id="7a4a2-112">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="7a4a2-113">Start-ManagedFolderAssistant-Identity<name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="7a4a2-113">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="7a4a2-114">Per ulteriori informazioni sulla configurazione di un criterio di archiviazione, vedere [set up an Archive and Deletion Policy for Mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="7a4a2-114">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  