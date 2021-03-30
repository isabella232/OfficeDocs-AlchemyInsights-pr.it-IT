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
ms.openlocfilehash: e69f3e529e4a2202f641cb62f42b1a20d774a398
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403747"
---
# <a name="workflow-is-not-starting"></a>Flusso di lavoro non avviato

- I flussi di lavoro di SharePoint 2010 e SharePoint 2013 non vengono avviati.

    - Se il flusso di lavoro non viene avviato, potrebbe verificarsi un problema temporaneo del servizio in cui gli utenti potrebbero subire ritardi intermittenti con l'avanzamento del flusso di lavoro. Controllare il [dashboard di integrità del](https://admin.microsoft.com/AdminPortal/Home/servicehealth) servizio per verificare se l'organizzazione è influenzata.

    - Se sono trascorse più di 24 ore dalla prima volta che hai visto questo problema, registra un ticket di supporto. In molti casi, stiamo già lavorando a una soluzione. Fornire almeno 24 ore per completare una soluzione.

- Flussi di lavoro di SharePoint 2010 ritardati all'avvio.

    - Ciò si verifica se il flusso di lavoro viene attivato in batch di grandi dimensioni. (ad esempio, quando vengono aggiunti più elementi contemporaneamente).

    - I flussi di lavoro non sono progettati per l'esecuzione in tempo reale, quindi un ritardo è in base alla progettazione.

   -  Se il flusso di lavoro è complesso XMOL (Extensible Object Markup Language), la compilazione può essere lenta. Controlla [questo](https://support.microsoft.com//kb/3043697) articolo.

    - È consigliabile semplificare il flusso di lavoro o riprogettare il flusso di lavoro utilizzando il tipo di piattaforma flusso di lavoro di Microsoft SharePoint 2013.

    - Se la cronologia del flusso di lavoro è aumentata, è possibile eliminare gli elementi o creare un nuovo elenco della cronologia.

        Ulteriori informazioni : [Eliminazione della cronologia del flusso di lavoro](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Argomenti correlati
Si desidera provare Microsoft Flow in SharePoint Online?
- [Create Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint e Flusso](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
