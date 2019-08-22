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
ms.openlocfilehash: 261fe1b1bc815dd4ad568051cfefad1e214b957e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36530882"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="1f73a-102">La posta elettronica del flusso di lavoro non viene inviata per un elenco o una raccolta di SharePoint</span><span class="sxs-lookup"><span data-stu-id="1f73a-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="1f73a-103">I messaggi di posta elettronica provenienti da flussi di lavoro non vengono inviati a tutti gli utenti o solo a utenti specifici oppure viene visualizzato l'errore che **il messaggio di posta elettronica non può inviare. Verificare che l'indirizzo di posta elettronica disponga di un destinatario valido**.</span><span class="sxs-lookup"><span data-stu-id="1f73a-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="1f73a-104">Controllare se l'utente è presente nel gruppo di autorizzazioni **tutti** gli utenti (elenco informazioni utente) per la raccolta siti.</span><span class="sxs-lookup"><span data-stu-id="1f73a-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="1f73a-105">URL diretto di esempio:<tenant>https://.<sitename>SharePoint.com/sites//_layouts/15/people.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="1f73a-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="1f73a-106">Se l'utente non esiste, verificare che l'utente sia connesso alla pagina.</span><span class="sxs-lookup"><span data-stu-id="1f73a-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="1f73a-107">Se si tratta di un utente esterno, verificare che l'invito sia stato accettato.</span><span class="sxs-lookup"><span data-stu-id="1f73a-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="1f73a-108">Se l'utente esiste nel gruppo autorizzazioni, verificare che l'indirizzo di posta elettronica sia corretto.</span><span class="sxs-lookup"><span data-stu-id="1f73a-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="1f73a-109">Se l'indirizzo di posta elettronica degli utenti non è impostato qui, creare un avviso di esempio per l'utente che forza la sincronizzazione dell'account utente da profili utente di SharePoint a questa raccolta siti.</span><span class="sxs-lookup"><span data-stu-id="1f73a-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="1f73a-110">La posta elettronica proveniente dai flussi di lavoro viene inviata agli amministratori della raccolta siti, ma non ad altri utenti e viene visualizzato il messaggio di errore **http Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.Utilities.Utility.SendEmail**.</span><span class="sxs-lookup"><span data-stu-id="1f73a-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="1f73a-111">Vedere [accesso negato quando si invia un messaggio di posta elettronica a un gruppo di SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="1f73a-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="1f73a-112">Verificare inoltre che la caratteristica di raccolta siti per la **modalità di blocco delle autorizzazioni utente con accesso limitato** non sia attiva.</span><span class="sxs-lookup"><span data-stu-id="1f73a-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="1f73a-113">Argomenti correlati</span><span class="sxs-lookup"><span data-stu-id="1f73a-113">Related topics</span></span>
<span data-ttu-id="1f73a-114">Si desidera provare Microsoft Flow in SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="1f73a-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="1f73a-115">Crea flusso</span><span class="sxs-lookup"><span data-stu-id="1f73a-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="1f73a-116">SharePoint e flusso</span><span class="sxs-lookup"><span data-stu-id="1f73a-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


