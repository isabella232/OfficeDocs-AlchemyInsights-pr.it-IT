---
title: Richiamare o sostituire un messaggio di posta elettronica
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: e541620a499b02a7206579ffcc505ceb4e632a4c
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742759"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a><span data-ttu-id="79944-102">Richiamare o sostituire un messaggio di posta elettronica in Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="79944-102">Recall or replace an email message in Microsoft 365</span></span>

- <span data-ttu-id="79944-103">È possibile **richiamare solo i messaggi inviati alle persone all'interno dell'organizzazione**.</span><span class="sxs-lookup"><span data-stu-id="79944-103">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="79944-104">Se il messaggio è stato inviato a un indirizzo Gmail, ad esempio, non è possibile richiamarlo.</span><span class="sxs-lookup"><span data-stu-id="79944-104">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="79944-105">È possibile **richiamare solo i messaggi inviati da Outlook 2016 per il PC**.</span><span class="sxs-lookup"><span data-stu-id="79944-105">You can **only recall messages sent from Outlook 2016 for the PC**.</span></span> <span data-ttu-id="79944-106">Se un utente invia un messaggio utilizzando Outlook per Mac o Outlook sul Web, non è possibile richiamarlo.</span><span class="sxs-lookup"><span data-stu-id="79944-106">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>
- <span data-ttu-id="79944-107">Se si è un amministratore, è possibile **richiamare i messaggi per conto degli utenti utilizzando PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="79944-107">If you're an admin, you can **recall messages on behalf of users by using PowerShell**.</span></span> <span data-ttu-id="79944-108">Non è possibile richiamare messaggi dall'interfaccia di amministrazione.</span><span class="sxs-lookup"><span data-stu-id="79944-108">You can't recall messages from the admin center.</span></span> <span data-ttu-id="79944-109">Scorrere verso il basso fino a "cercare ed eliminare i messaggi di posta elettronica nell'organizzazione" per ulteriori informazioni.</span><span class="sxs-lookup"><span data-stu-id="79944-109">Scroll down to "Search for and delete email messages in your organization" for more information.</span></span>

<span data-ttu-id="79944-110">**Richiamare o sostituire un messaggio di posta elettronica inviato**</span><span class="sxs-lookup"><span data-stu-id="79944-110">**Recall or replace an email message that you sent**</span></span>

1. <span data-ttu-id="79944-111">Nel riquadro delle cartelle nella parte sinistra della finestra di Outlook scegliere la cartella posta inviata.</span><span class="sxs-lookup"><span data-stu-id="79944-111">In the folder pane on the left of the Outlook window, choose the Sent Items folder.</span></span>
2. <span data-ttu-id="79944-112">Aprire il messaggio che si desidera richiamare.</span><span class="sxs-lookup"><span data-stu-id="79944-112">Open the message that you want to recall.</span></span> <span data-ttu-id="79944-113">È necessario fare doppio clic per aprire il messaggio.</span><span class="sxs-lookup"><span data-stu-id="79944-113">You must double-click to open the message.</span></span> <span data-ttu-id="79944-114">Se si seleziona il messaggio in modo che venga visualizzato nel riquadro di lettura, non sarà possibile richiamare il messaggio.</span><span class="sxs-lookup"><span data-stu-id="79944-114">Selecting the message so it appears in the reading pane won't allow you to recall the message.</span></span>
3. <span data-ttu-id="79944-115">Nella scheda messaggio, selezionare **azioni** > **richiamare questo messaggio**.</span><span class="sxs-lookup"><span data-stu-id="79944-115">From the Message tab, select **Actions** > **Recall This Message**.</span></span>
4. <span data-ttu-id="79944-116">Scegliere **Elimina copie non lette del messaggio** o **Elimina copie non lette e Sostituisci con un nuovo messaggio**, quindi selezionare **OK**.</span><span class="sxs-lookup"><span data-stu-id="79944-116">Choose **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, then select **OK**.</span></span>
5. <span data-ttu-id="79944-117">Se si sta inviando un messaggio di sostituzione, comporre il messaggio, quindi selezionare **Invia**.</span><span class="sxs-lookup"><span data-stu-id="79944-117">If you're sending a replacement message, compose the message, then select **Send**.</span></span>
6. <span data-ttu-id="79944-118">L'esito positivo o negativo di un messaggio di richiamo dipende dalle impostazioni dei destinatari in Outlook.</span><span class="sxs-lookup"><span data-stu-id="79944-118">The success or failure of a message recall depends on the recipients' settings in Outlook.</span></span>

<span data-ttu-id="79944-119">Per ulteriori informazioni, tra cui la verifica del richiamo, vedere [Recall or Replace an email message you sent](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="79944-119">For more information, including how to check on the recall, see [Recall or replace an email message that you sent](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="79944-120">***Cercare ed eliminare i messaggi di posta elettronica nell'organizzazione*** Per cercare ed eliminare i messaggi di posta elettronica nell'organizzazione, è più semplice se si è un amministratore globale. Se non si è un amministratore globale, è necessario aggiungere l'account al gruppo di ruoli di eDiscovery Manager o al ruolo di gestione della ricerca di conformità.</span><span class="sxs-lookup"><span data-stu-id="79944-120">***Search for and delete email messages in your organization*** To search for and delete email messages in your organization, it's easiest if you're a global admin. If you're not a global admin, your account must be added to the eDiscovery Manager role group, or to the Compliance Search management role.</span></span> <span data-ttu-id="79944-121">Per eliminare i messaggi, è necessario aggiungere il gruppo di ruoli Gestione organizzazione o il ruolo di gestione ricerca e Purge.</span><span class="sxs-lookup"><span data-stu-id="79944-121">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="79944-122">Le autorizzazioni per questi ruoli vengono assegnate al [Centro sicurezza & Compliance](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="79944-122">Permissions to these roles are assigned in the [Security & compliance center](https://protection.office.com/).</span></span>

1. <span data-ttu-id="79944-123">[Creare una ricerca di contenuto](https://docs.microsoft.com/office365/securitycompliance/content-search) per trovare il messaggio da eliminare.</span><span class="sxs-lookup"><span data-stu-id="79944-123">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
2. <span data-ttu-id="79944-124">[Connettersi a PowerShell in Centro sicurezza e conformità](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="79944-124">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span> 

<span data-ttu-id="79944-125">Se si utilizza l'autenticazione Master, vedere [Connect to Microsoft 365 security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="79944-125">If you're using MFA, see [Connect to Microsoft 365 security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span> 
