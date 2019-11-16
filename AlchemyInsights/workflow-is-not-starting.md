---
title: Il flusso di lavoro non inizia
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 8/2/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 2d85dcf9111d48cb529c583c733823b404eb3188
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/15/2019
ms.locfileid: "36738093"
---
# <a name="workflow-is-not-starting"></a>Il flusso di lavoro non inizia

- I flussi di lavoro di SharePoint 2010 e SharePoint 2013 non vengono avviati.

    - Se il flusso di lavoro non è avviato, potrebbe verificarsi un problema di servizio temporaneo in cui gli utenti potrebbero riscontrare ritardi intermittenti con lo stato del flusso di lavoro. Controllare il [Dashboard dell'integrità del servizio](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) per verificare se l'organizzazione ha un impatto.

    - Se sono passate più di 24 ore da quando hai visto questo problema, registra un ticket di supporto. In molti casi, stiamo già lavorando a una soluzione. Per completare una soluzione, è possibile fornirci almeno 24 ore.

- I flussi di lavoro di SharePoint 2010 sono stati posticipati all'inizio.

    - Questo problema si verifica se il flusso di lavoro viene attivato in batch di grandi dimensioni. ad esempio, quando vengono aggiunti contemporaneamente più elementi.

    - I flussi di lavoro non sono stati creati per l'esecuzione in tempo reale, quindi un ritardo è in base alla progettazione.

   -  Se il flusso di lavoro è XMOL (Extensible Object Markup Language) complesso, la compilazione può essere lenta. Controllare [questo](https://support.microsoft.com//kb/3043697) articolo.

    - È consigliabile semplificare il flusso di lavoro o riprogettarlo utilizzando il tipo di piattaforma per flussi di lavoro di Microsoft SharePoint 2013.

    - Se la cronologia del flusso di lavoro è cresciuta, potrebbe essere necessario eliminare gli elementi o creare un nuovo elenco di cronologia.

        Ulteriori informazioni: [eliminare la cronologia dei flussi di lavoro](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Argomenti correlati
Si desidera provare Microsoft Flow in SharePoint Online?
- [Crea flusso](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint e flusso](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


