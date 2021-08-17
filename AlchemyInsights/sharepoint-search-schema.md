---
title: Gestire lo schema di ricerca in SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 8eb0e93ea5bbf2154213274041b28a3c908090dae724b8f8e55fa2fb05f16d86
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54085088"
---
# <a name="manage-search-schema-in-sharepoint-online"></a>Gestire lo schema di ricerca in SharePoint Online

Lo schema di ricerca controlla quali utenti possono cercare, come gli utenti possono eseguire ricerche e come è possibile presentare i risultati nei siti Web di ricerca. 

Vedere [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) per informazioni su come: 
- Modificare lo schema di ricerca.
- Creare proprietà gestite.
- Mappare le proprietà sottoposte a ricerca per indicizzazione mappate alle proprietà gestite.

Tenere presente quanto segue per quanto riguarda la gestione dello schema di ricerca:

- Se viene visualizzato un  avviso che indica che l'applicazione viene sospesa quando si apporta una modifica allo schema, questa operazione è temporanea solo in quanto è in corso la manutenzione del servizio. 

    Se sono trascorse più di 24 ore e l'avviso persiste, registrare un caso di supporto.
- Quando si modificano proprietà gestite o si aggiungono nuove proprietà, le modifiche vengono applicate solo dopo la nuova ricerca per indicizzazione del contenuto. In SharePoint Online, la ricerca per indicizzazione viene eseguita automaticamente in base alla pianificazione della ricerca per indicizzazione definita.
- Per assicurarsi che le modifiche siano sottoposte a ricerca per indicizzazione, è possibile richiedere in modo specifico una nuova [indicizzazione dell'elenco o della raccolta](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list) 

Per una panoramica completa dello schema di ricerca, vedere [Introduzione allo schema di ricerca](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/) 


