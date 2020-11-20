---
title: Richiamare o sostituire un messaggio di posta elettronica
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 05016213a1387c5290cb5899359f1f10b5a413c0
ms.sourcegitcommit: 4e0ae808ee2a586339b396320e3edb8ba066a91a
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/19/2020
ms.locfileid: "49353510"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a><span data-ttu-id="afd90-102">Richiamare o sostituire un messaggio di posta elettronica in Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="afd90-102">Recall or replace an email message in Microsoft 365</span></span>

- <span data-ttu-id="afd90-103">È possibile **richiamare solo i messaggi inviati alle persone all'interno dell'organizzazione**.</span><span class="sxs-lookup"><span data-stu-id="afd90-103">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="afd90-104">Ad esempio, se il messaggio è stato inviato a un indirizzo Gmail, non è possibile richiamarlo.</span><span class="sxs-lookup"><span data-stu-id="afd90-104">For example, if the message was sent to a Gmail address, you can't recall it.</span></span>
- <span data-ttu-id="afd90-105">È possibile **richiamare solo i messaggi inviati da Outlook per il PC**.</span><span class="sxs-lookup"><span data-stu-id="afd90-105">You can **only recall messages sent from Outlook for the PC**.</span></span> <span data-ttu-id="afd90-106">Se un utente invia un messaggio utilizzando Outlook per Mac o Outlook sul Web, non è possibile richiamarlo.</span><span class="sxs-lookup"><span data-stu-id="afd90-106">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>
- <span data-ttu-id="afd90-107">In qualità di amministratore tenant, è possibile **richiamare i messaggi per conto degli utenti utilizzando PowerShell** (per ulteriori informazioni, vedere: [cercare ed eliminare i messaggi di posta elettronica](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).</span><span class="sxs-lookup"><span data-stu-id="afd90-107">As a tenant administrator, you can **recall messages on behalf of users by using PowerShell** (For more information, see: [Search for and delete email messages](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).</span></span>
- <span data-ttu-id="afd90-108">Non è possibile richiamare messaggi dall'interfaccia di amministrazione.</span><span class="sxs-lookup"><span data-stu-id="afd90-108">You can't recall messages from the admin center.</span></span> <span data-ttu-id="afd90-109">Scorrere verso il basso fino a "cercare ed eliminare i messaggi di posta elettronica nell'organizzazione" per ulteriori informazioni.</span><span class="sxs-lookup"><span data-stu-id="afd90-109">Scroll down to "Search for and delete email messages in your organization" for more information.</span></span>

<span data-ttu-id="afd90-110">**Richiamare o sostituire un messaggio di posta elettronica inviato**</span><span class="sxs-lookup"><span data-stu-id="afd90-110">**Recall or replace an email message that you sent**</span></span>

1. <span data-ttu-id="afd90-111">Nel riquadro delle cartelle nella parte sinistra della finestra di Outlook scegliere la cartella posta inviata.</span><span class="sxs-lookup"><span data-stu-id="afd90-111">In the folder pane on the left of the Outlook window, choose the Sent Items folder.</span></span>
2. <span data-ttu-id="afd90-112">Aprire il messaggio che si desidera richiamare.</span><span class="sxs-lookup"><span data-stu-id="afd90-112">Open the message that you want to recall.</span></span> <span data-ttu-id="afd90-113">È necessario fare doppio clic per aprire il messaggio.</span><span class="sxs-lookup"><span data-stu-id="afd90-113">You must double-click to open the message.</span></span> <span data-ttu-id="afd90-114">Se si seleziona il messaggio in modo che venga visualizzato nel riquadro di lettura, non sarà possibile richiamare il messaggio.</span><span class="sxs-lookup"><span data-stu-id="afd90-114">Selecting the message so it appears in the reading pane won't allow you to recall the message.</span></span>
3. <span data-ttu-id="afd90-115">Nella scheda messaggio, selezionare **azioni**  >  **richiamare questo messaggio**.</span><span class="sxs-lookup"><span data-stu-id="afd90-115">From the Message tab, select **Actions** > **Recall This Message**.</span></span>
4. <span data-ttu-id="afd90-116">Scegliere **Elimina copie non lette del messaggio** o **Elimina copie non lette e Sostituisci con un nuovo messaggio**, quindi selezionare **OK**.</span><span class="sxs-lookup"><span data-stu-id="afd90-116">Choose **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, then select **OK**.</span></span>
5. <span data-ttu-id="afd90-117">Se si sta inviando un messaggio di sostituzione, comporre il messaggio, quindi selezionare **Invia**.</span><span class="sxs-lookup"><span data-stu-id="afd90-117">If you're sending a replacement message, compose the message, then select **Send**.</span></span>
6. <span data-ttu-id="afd90-118">L'esito positivo o negativo di un messaggio di richiamo dipende dalle impostazioni dei destinatari in Outlook.</span><span class="sxs-lookup"><span data-stu-id="afd90-118">The success or failure of a message recall depends on the recipients' settings in Outlook.</span></span>

<span data-ttu-id="afd90-119">Per ulteriori informazioni, tra cui la verifica del richiamo, vedere [Recall or Replace an email message you sent](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="afd90-119">For more information, including how to check on the recall, see [Recall or replace an email message that you sent](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="afd90-120">**_Per cercare ed eliminare i messaggi di posta elettronica nell'organizzazione_**, è più semplice se si è un amministratore globale. Se non si è un amministratore globale, è necessario aggiungere l'account al gruppo di ruoli di eDiscovery Manager o al ruolo di gestione della ricerca di conformità.</span><span class="sxs-lookup"><span data-stu-id="afd90-120">**_To search for and delete email messages in your organization_**, it's easiest if you're a global admin. If you're not a global admin, your account must be added to the eDiscovery Manager role group, or to the Compliance Search management role.</span></span> <span data-ttu-id="afd90-121">Per eliminare i messaggi, è necessario aggiungere il gruppo di ruoli Gestione organizzazione o il ruolo di gestione ricerca e Purge.</span><span class="sxs-lookup"><span data-stu-id="afd90-121">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="afd90-122">Le autorizzazioni per questi ruoli vengono assegnate al [Centro sicurezza & Compliance](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="afd90-122">Permissions to these roles are assigned in the [Security & compliance center](https://protection.office.com/).</span></span>

1. <span data-ttu-id="afd90-123">[Creare una ricerca di contenuto](https://docs.microsoft.com/microsoft-365/compliance/content-search) per trovare il messaggio da eliminare.</span><span class="sxs-lookup"><span data-stu-id="afd90-123">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
2. <span data-ttu-id="afd90-124">[Connettersi a PowerShell in Centro sicurezza e conformità](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="afd90-124">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span>

<span data-ttu-id="afd90-125">Se si utilizza l'autenticazione a più fattori, vedere [Connect to Microsoft 365 Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="afd90-125">If you're using MFA (multi-factor authentication), see [Connect to Microsoft 365 Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).</span></span>
