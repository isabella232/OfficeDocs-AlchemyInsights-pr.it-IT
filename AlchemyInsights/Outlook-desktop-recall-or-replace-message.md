---
title: Outlook desktop richiamare o sostituire un messaggio di posta elettronica
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 3d3a6c253317137b7069a978b907c97d61bf7313
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36496115"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="d760c-102">Richiamare o sostituire un messaggio di posta elettronica di Outlook</span><span class="sxs-lookup"><span data-stu-id="d760c-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="d760c-103">Come amministratore, è possibile **richiamare i messaggi per conto di utenti che utilizzano PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="d760c-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="d760c-104">Non è possibile richiamare messaggi dall'interfaccia di amministrazione.</span><span class="sxs-lookup"><span data-stu-id="d760c-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="d760c-105">È possibile **richiamare solo i messaggi inviati alle persone all'interno dell'organizzazione**.</span><span class="sxs-lookup"><span data-stu-id="d760c-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="d760c-106">Se il messaggio è stato inviato a un indirizzo Gmail, ad esempio, non è possibile richiamarlo.</span><span class="sxs-lookup"><span data-stu-id="d760c-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="d760c-107">È possibile **richiamare solo i messaggi inviati da Outlook 2016 sul PC**.</span><span class="sxs-lookup"><span data-stu-id="d760c-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="d760c-108">Se un utente invia un messaggio utilizzando Outlook per Mac o Outlook sul Web, non è possibile richiamarlo.</span><span class="sxs-lookup"><span data-stu-id="d760c-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="d760c-109">Per richiamare o sostituire un messaggio di posta elettronica:</span><span class="sxs-lookup"><span data-stu-id="d760c-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="d760c-110">Nel riquadro delle cartelle nella parte sinistra della finestra di Outlook selezionare la cartella posta inviata.</span><span class="sxs-lookup"><span data-stu-id="d760c-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="d760c-111">Fare doppio clic sul messaggio che si desidera richiamare per aprirlo.</span><span class="sxs-lookup"><span data-stu-id="d760c-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="d760c-112">Selezionare la scheda **messaggio** e quindi fare clic su **azioni** > **richiamare questo messaggio**.</span><span class="sxs-lookup"><span data-stu-id="d760c-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="d760c-113">Selezionare **Elimina copie non lette del messaggio** o **Elimina copie non lette e Sostituisci con un nuovo messaggio**e quindi fare clic su **OK**.</span><span class="sxs-lookup"><span data-stu-id="d760c-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="d760c-114">Se si sta inviando un messaggio di sostituzione, comporre il messaggio, quindi selezionare **Invia**.</span><span class="sxs-lookup"><span data-stu-id="d760c-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="d760c-115">L'esito positivo o negativo di un messaggio di richiamo dipende dalle impostazioni del destinatario in Outlook.</span><span class="sxs-lookup"><span data-stu-id="d760c-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="d760c-116">Per la procedura da eseguire per la verifica del richiamo, vedere [questo articolo](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="d760c-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="d760c-117">Cercare ed eliminare i messaggi di posta elettronica nell'organizzazione</span><span class="sxs-lookup"><span data-stu-id="d760c-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="d760c-118">Se non si è un amministratore globale, è necessario aggiungere l'account al ruolo eDiscovery Manager o alla funzione di gestione della ricerca di conformità per cercare i messaggi.</span><span class="sxs-lookup"><span data-stu-id="d760c-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="d760c-119">Per eliminare i messaggi, è necessario aggiungere il gruppo di ruoli Gestione organizzazione o il ruolo di gestione ricerca e Purge.</span><span class="sxs-lookup"><span data-stu-id="d760c-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="d760c-120">Le autorizzazioni per questi ruoli vengono assegnate al [Centro sicurezza e conformità](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="d760c-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="d760c-121">[Creare una ricerca di contenuto](https://docs.microsoft.com/office365/securitycompliance/content-search) per trovare il messaggio da eliminare.</span><span class="sxs-lookup"><span data-stu-id="d760c-121">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="d760c-122">[Connettersi a PowerShell per Centro sicurezza e conformità](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="d760c-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="d760c-123">Se si utilizza l'autenticazione a più fattori, vedere [Connect to Office 365 Security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="d760c-123">If you're using multi-factor authentication, see [Connect to Office 365 Security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>