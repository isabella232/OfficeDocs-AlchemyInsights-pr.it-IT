---
title: Spostare i messaggi di posta elettronica nella cassetta postale di archiviazione
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
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 61d0b1a58fff6655b745bb9d39e8384f0a543336
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799784"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="8b8fb-102">Spostare la posta elettronica nella cassetta postale di archiviazione</span><span class="sxs-lookup"><span data-stu-id="8b8fb-102">Move email to the archive mailbox</span></span>

<span data-ttu-id="8b8fb-103">Se si desidera che vengano eseguiti controlli automatici per le impostazioni indicate di seguito, selezionare il pulsante indietro <--nella parte superiore di questa pagina e quindi immettere l'indirizzo di posta elettronica dell'utente che ha problemi a spostare la posta elettronica nella cassetta postale di archiviazione.</span><span class="sxs-lookup"><span data-stu-id="8b8fb-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems moving email to their archive mailbox.</span></span>

1. <span data-ttu-id="8b8fb-104">Verificare che sia stata abilitata una **cassetta postale di archiviazione** .</span><span class="sxs-lookup"><span data-stu-id="8b8fb-104">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="8b8fb-105">In caso contrario, utilizzare la procedura descritta in [questo articolo](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) per abilitare la cassetta postale di archiviazione.</span><span class="sxs-lookup"><span data-stu-id="8b8fb-105">If not, use the steps in [this article](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="8b8fb-106">Per archiviare automaticamente i messaggi nella cassetta postale di archiviazione, è necessario impostare un tag di conservazione con l'azione **Sposta nell'archivio** su **applicato automaticamente all'intero tag della cassetta postale (impostazione predefinita)**.</span><span class="sxs-lookup"><span data-stu-id="8b8fb-106">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="8b8fb-107">Utilizzare la procedura seguente per creare il tag: [archivio predefinito](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag)tag.</span><span class="sxs-lookup"><span data-stu-id="8b8fb-107">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="8b8fb-108">Successivamente, aggiungere il tag di **archiviazione** al criterio di conservazione.</span><span class="sxs-lookup"><span data-stu-id="8b8fb-108">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="8b8fb-109">Nell'interfaccia di amministrazione di Exchange, scegliere **criteri di conservazione** > aggiungere il **tag Move to Archive** al criterio > **Save**.</span><span class="sxs-lookup"><span data-stu-id="8b8fb-109">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="8b8fb-110">A questo punto, [assegnare il criterio di conservazione](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) alla cassetta postale dell'utente specifico.</span><span class="sxs-lookup"><span data-stu-id="8b8fb-110">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="8b8fb-111">Lo stesso criterio verrà applicato sia alla cassetta postale **principale** che a quella di **archiviazione** .</span><span class="sxs-lookup"><span data-stu-id="8b8fb-111">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="8b8fb-112">Potrebbe essere necessario forzare l'esecuzione dell'Assistente cartelle gestite e applicare le nuove impostazioni alla cassetta postale dell'utente.</span><span class="sxs-lookup"><span data-stu-id="8b8fb-112">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="8b8fb-113">Eseguire il seguente comando quando [si è connessi a Exo PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) per avviare l'Assistente cartelle gestite per una cassetta postale specifica:</span><span class="sxs-lookup"><span data-stu-id="8b8fb-113">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="8b8fb-114">Start-ManagedFolderAssistant-Identity <name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="8b8fb-114">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="8b8fb-115">Per ulteriori informazioni sulla configurazione di un criterio di archiviazione, vedere [set up an Archive and Deletion Policy for Mailboxes](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="8b8fb-115">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  