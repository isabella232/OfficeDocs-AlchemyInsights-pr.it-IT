---
title: I messaggi di posta elettronica del flusso di lavoro non vengono inviati
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 2caf8e0878da0049667d9a19f4488eaec4b9327fbf36be7d29dbf4b7a9c89158
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072524"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>La posta elettronica del flusso di lavoro non viene inviata per un SharePoint o una raccolta

1. I messaggi di posta elettronica provenienti dai flussi di lavoro non vengono inviati a tutti gli utenti o solo a utenti specifici oppure viene visualizzato l'errore Impossibile inviare il messaggio di posta elettronica. Verificare che il messaggio di posta elettronica abbia un **destinatario valido.**

    Verificare se l'utente è presente nel **gruppo di** autorizzazioni Tutti gli utenti (elenco di informazioni utente) per la raccolta siti.  URL diretto di esempio: https:// <tenant> .sharepoint.com/sites/ <sitename> /_layouts/15/people.aspx? MembershipGroupId=0

    - Se l'utente non esiste, verificare che l'utente sia connesso alla pagina. 
    - Se si tratta di un utente esterno, assicurarsi che l'invito sia stato accettato.
    - Se l'utente esiste nel gruppo di autorizzazioni, verificare che l'indirizzo di posta elettronica sia corretto.
    - Se l'indirizzo di posta elettronica degli utenti non è impostato qui, creare un avviso di esempio per tale utente che forza la sincronizzazione dell'account utente dai profili utente di SharePoint a questa raccolta siti.
 
2. I messaggi di posta elettronica provenienti dai flussi di lavoro vengono inviati agli amministratori della raccolta siti ma non ad altri utenti e viene visualizzato l'errore HTTP Accesso negato a **<span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.
 

    Vedere [Accesso negato quando si invia un messaggio](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups)di posta elettronica a SharePoint gruppo .

    Verificare inoltre che la **caratteristica Della raccolta** siti in modalità di blocco delle autorizzazioni utente con accesso limitato non sia attiva.


## <a name="related-topics"></a>Argomenti correlati
Vuoi provare a Microsoft Flow in SharePoint Online?
- [Creare Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint e Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


