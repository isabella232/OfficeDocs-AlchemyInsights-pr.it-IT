---
title: Flusso di lavoro non avviato
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
- "9000144"
- "1670"
ms.openlocfilehash: 77a3c022a9a3a82041b4a4a70c72c2e0940c0fba27f296f07881e3abebf1e464
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53907742"
---
# <a name="workflow-is-not-starting"></a>Flusso di lavoro non avviato

- SharePoint 2010 e SharePoint 2013 non vengono avviati.

    - Se il flusso di lavoro non viene avviato, potrebbe verificarsi un problema temporaneo del servizio in cui gli utenti potrebbero subire ritardi intermittenti con l'avanzamento del flusso di lavoro. Controllare il [dashboard di integrità del](https://admin.microsoft.com/AdminPortal/Home/servicehealth) servizio per verificare se l'organizzazione è influenzata.

    - Se sono trascorse più di 24 ore dalla prima volta che hai visto questo problema, registra un ticket di supporto. In molti casi, stiamo già lavorando a una soluzione. Fornire almeno 24 ore per completare una soluzione.

- SharePoint flussi di lavoro 2010 ritardati all'avvio.

    - Ciò si verifica se il flusso di lavoro viene attivato in batch di grandi dimensioni. (ad esempio, quando vengono aggiunti più elementi contemporaneamente).

    - I flussi di lavoro non sono progettati per l'esecuzione in tempo reale, quindi un ritardo è in base alla progettazione.

   -  Se il flusso di lavoro è complesso XMOL (Extensible Object Markup Language), la compilazione può essere lenta. Controlla [questo](https://support.microsoft.com//kb/3043697) articolo.

    - È consigliabile semplificare il flusso di lavoro o riprogettare il flusso di lavoro utilizzando il tipo di piattaforma Microsoft SharePoint 2013 Workflow.

    - Se la cronologia del flusso di lavoro è aumentata, è possibile eliminare gli elementi o creare un nuovo elenco della cronologia.

        Ulteriori informazioni : [Eliminazione della cronologia del flusso di lavoro](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Argomenti correlati
Vuoi provare a Microsoft Flow in SharePoint Online?
- [Creare Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint e Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
