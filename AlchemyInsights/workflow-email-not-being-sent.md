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
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>La posta elettronica del flusso di lavoro non viene inviata per un elenco o una raccolta di SharePoint

1. I messaggi di posta elettronica provenienti da flussi di lavoro non vengono inviati a tutti gli utenti o solo a utenti specifici oppure viene visualizzato l'errore che **il messaggio di posta elettronica non può inviare. Verificare che l'indirizzo di posta elettronica disponga di un destinatario valido**.

    Controllare se l'utente è presente nel gruppo di autorizzazioni **tutti** gli utenti (elenco informazioni utente) per la raccolta siti.  URL diretto di esempio:<tenant>https://.<sitename>SharePoint.com/sites//_layouts/15/people.aspx? MembershipGroupId = 0

    - Se l'utente non esiste, verificare che l'utente sia connesso alla pagina. 
    - Se si tratta di un utente esterno, verificare che l'invito sia stato accettato.
    - Se l'utente esiste nel gruppo autorizzazioni, verificare che l'indirizzo di posta elettronica sia corretto.
    - Se l'indirizzo di posta elettronica degli utenti non è impostato qui, creare un avviso di esempio per l'utente che forza la sincronizzazione dell'account utente da profili utente di SharePoint a questa raccolta siti.
 
2. La posta elettronica proveniente dai flussi di lavoro viene inviata agli amministratori della raccolta siti, ma non ad altri utenti e viene visualizzato il messaggio di errore **http Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.Utilities.Utility.SendEmail**.
 

    Vedere [accesso negato quando si invia un messaggio di posta elettronica a un gruppo di SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Verificare inoltre che la caratteristica di raccolta siti per la **modalità di blocco delle autorizzazioni utente con accesso limitato** non sia attiva.


## <a name="related-topics"></a>Argomenti correlati
Si desidera provare Microsoft Flow in SharePoint Online?
- [Crea flusso](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint e flusso](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


