---
title: Commenti in Microsoft Planner
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001717"
- "3810"
ms.openlocfilehash: 048b63619256c1322837a06115f97127188aec6d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47793582"
---
# <a name="comments-in-microsoft-planner"></a><span data-ttu-id="6d74e-102">Commenti in Microsoft Planner</span><span class="sxs-lookup"><span data-stu-id="6d74e-102">Comments in Microsoft Planner</span></span>

<span data-ttu-id="6d74e-103">I commenti relativi alle attività nell'ambito di un piano vengono archiviati nella cassetta postale di Exchange Online relativa al gruppo di Microsoft 365 associato al piano.</span><span class="sxs-lookup"><span data-stu-id="6d74e-103">Comments for tasks within a plan are stored in the Exchange Online mailbox for the Microsoft 365 Group associated with the plan.</span></span>  <span data-ttu-id="6d74e-104">Quando si pubblica un commento su un'attività, viene inviata una notifica tramite posta elettronica alla cartella posta in arrivo del gruppo, che riceverà un messaggio di posta elettronica per ogni commento successivo.</span><span class="sxs-lookup"><span data-stu-id="6d74e-104">When you post a comment on a task, an email notification is sent to the group inbox, and you will receive an email for each subsequent comment made on that task.</span></span>

<span data-ttu-id="6d74e-105">Ecco alcune risposte ai problemi comuni relativi ai commenti:</span><span class="sxs-lookup"><span data-stu-id="6d74e-105">Here are some answers to common issues related to comments:</span></span>

- <span data-ttu-id="6d74e-106">**Gli utenti non ricevono messaggi di posta elettronica**: i commenti vengono inviati alla posta in arrivo del gruppo a cui appartiene il piano.</span><span class="sxs-lookup"><span data-stu-id="6d74e-106">**Users are not receiving emails** - Comments are sent to the group inbox for the group the plan belongs to.</span></span> <span data-ttu-id="6d74e-107">Perché un utente riceva i messaggi di posta elettronica di gruppo, il gruppo deve essere configurato per l'invio delle conversazioni di gruppo alle cartelle posta in arrivo dei membri.</span><span class="sxs-lookup"><span data-stu-id="6d74e-107">For a user to receive group emails, the group should be configured to send group conversations to member's inboxes.</span></span>

- <span data-ttu-id="6d74e-108">**I commenti non vengono salvati**: l'utente che aggiunge il commento non è autorizzato a inviare messaggi di posta elettronica al gruppo di Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="6d74e-108">**Comments are not getting saved** -  The user adding the comment does not have permission to send email to the Microsoft 365 group.</span></span> <span data-ttu-id="6d74e-109">Per altre informazioni su questo scenario, leggere l'articolo sul [funzionamento di Microsoft Planner](https://techcommunity.microsoft.com/t5/planner-blog/how-microsoft-planner-works/ba-p/1214736).</span><span class="sxs-lookup"><span data-stu-id="6d74e-109">Read [How Microsoft Planner Works](https://techcommunity.microsoft.com/t5/planner-blog/how-microsoft-planner-works/ba-p/1214736) for more information about this scenario.</span></span>

- <span data-ttu-id="6d74e-110">Viene visualizzato il messaggio di errore **Non hai più accesso** oppure **gli utenti ospiti non riescono ad aggiungere commenti**: gli utenti ospiti che non possono inviare messaggi di posta elettronica alla cartella posta in arrivo del gruppo potrebbero visualizzare questo messaggio.</span><span class="sxs-lookup"><span data-stu-id="6d74e-110">The error **You no longer have access** is displayed, or **guest users are unable to add comments** - Guest users who cannot send e-mail to the group inbox may see this message.</span></span> <span data-ttu-id="6d74e-111">Per risolvere il problema, verificare che l'utente ospite abbia un indirizzo di posta elettronica valido.</span><span class="sxs-lookup"><span data-stu-id="6d74e-111">To resolve, ensure that the guest user has a valid e-mail address.</span></span>

- <span data-ttu-id="6d74e-112">**Gli utenti rimossi ricevono i messaggi di posta elettronica**: se un utente invia un commento a un'attività prima di essere rimosso dal piano, il thread di posta elettronica includerà l'utente per ogni commento aggiunto all'attività.</span><span class="sxs-lookup"><span data-stu-id="6d74e-112">**Removed users are getting emails** -  If a user comments on a task prior to being removed from the plan, the email thread includes the user for each comment made on the task.</span></span>

<span data-ttu-id="6d74e-113">Per informazioni dettagliate sui commenti con Microsoft Planner, vedere l'articolo sul [funzionamento di Microsoft Planner](https://techcommunity.microsoft.com/t5/planner-blog/how-microsoft-planner-works/ba-p/1214736) e [Commentare le attività in Microsoft Planner](https://support.microsoft.com/office/fd4aedde-7785-4cd0-96ee-122fbc9140e1).</span><span class="sxs-lookup"><span data-stu-id="6d74e-113">For detailed information on comments with Microsoft Planner, see [how Microsoft Planner works](https://techcommunity.microsoft.com/t5/planner-blog/how-microsoft-planner-works/ba-p/1214736) and [Comment on tasks in Microsoft Planner](https://support.microsoft.com/office/fd4aedde-7785-4cd0-96ee-122fbc9140e1).</span></span>
