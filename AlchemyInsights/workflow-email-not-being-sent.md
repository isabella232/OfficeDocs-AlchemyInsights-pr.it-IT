---
title: La posta elettronica del flusso di lavoro non viene inviata
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 49c510668f4c73a71495b89ee9f810d4e7244da3
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270676"
---
# <a name="workflow-email-is-not-being-sent"></a><span data-ttu-id="f1221-102">La posta elettronica del flusso di lavoro non viene inviata</span><span class="sxs-lookup"><span data-stu-id="f1221-102">Workflow email is not being sent</span></span>

1. <span data-ttu-id="f1221-103">I messaggi di posta elettronica provenienti da flussi di lavoro non vengono inviati a tutti gli utenti o solo a utenti specifici oppure viene visualizzato l'errore che **il messaggio di posta elettronica non può inviare. Verificare che l'indirizzo di posta elettronica disponga di un destinatario valido**.</span><span class="sxs-lookup"><span data-stu-id="f1221-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="f1221-104">Controllare se l'utente è presente nel gruppo di autorizzazioni **tutti** gli utenti (elenco informazioni utente) per la raccolta siti.</span><span class="sxs-lookup"><span data-stu-id="f1221-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="f1221-105">URL diretto di esempio:<tenant>https://.<sitename>SharePoint.com/sites//_layouts/15/people.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="f1221-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="f1221-106">Se l'utente non esiste, verificare che l'utente sia connesso alla pagina.</span><span class="sxs-lookup"><span data-stu-id="f1221-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="f1221-107">Se si tratta di un utente esterno, verificare che l'invito sia stato accettato.</span><span class="sxs-lookup"><span data-stu-id="f1221-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="f1221-108">Se l'utente esiste nel gruppo autorizzazioni, verificare che l'indirizzo di posta elettronica sia corretto.</span><span class="sxs-lookup"><span data-stu-id="f1221-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="f1221-109">Se l'indirizzo di posta elettronica degli utenti non è impostato qui, creare un avviso di esempio per l'utente che forza la sincronizzazione dell'account utente da profili utente di SharePoint a questa raccolta siti.</span><span class="sxs-lookup"><span data-stu-id="f1221-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="f1221-110">La posta elettronica proveniente dai flussi di lavoro viene inviata agli amministratori della raccolta siti, ma non ad altri utenti e visualizza il messaggio <spam> <spam> \*\* <spam> <spam>di errore http vietato \*\*.</span><span class="sxs-lookup"><span data-stu-id="f1221-110">Email from Workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <spam><spam>https://URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**<spam><spam>.</span></span>
 

    <span data-ttu-id="f1221-111">Vedere [accesso negato quando si inviano messaggi di posta elettronica ai gruppi](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="f1221-111">See [Access Denied when sent email to groups](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="f1221-112">Verificare inoltre che la caratteristica di raccolta siti per la **modalità di blocco delle autorizzazioni utente con accesso limitato** non sia attiva.</span><span class="sxs-lookup"><span data-stu-id="f1221-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="f1221-113">Argomenti correlati</span><span class="sxs-lookup"><span data-stu-id="f1221-113">Related topics</span></span>
<span data-ttu-id="f1221-114">Si desidera provare Microsoft Flow in SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="f1221-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="f1221-115">Crea flusso</span><span class="sxs-lookup"><span data-stu-id="f1221-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="f1221-116">SharePoint e flusso</span><span class="sxs-lookup"><span data-stu-id="f1221-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


