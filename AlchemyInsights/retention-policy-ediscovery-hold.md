---
title: 2609-conservazione-o-eDiscovery-Hold
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2609"
- "9000048"
ms.openlocfilehash: 85c41995545efd8e1526d9f7dce4a23929f85be5
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994074"
---
# <a name="unable-to-delete-items-in-sharepoint-online-or-onedrive-for-business"></a>Impossibile eliminare gli elementi in SharePoint Online o OneDrive for business

L'utente o gli utenti potrebbero non essere in grado di eliminare gli elementi in SharePoint Online o OneDrive for business perché un criterio di conservazione, un'etichetta di conservazione o un blocco eDiscovery viene applicato a un SharePoint del sito di OneDrive o a un elemento specifico. Ciò include la possibilità di eliminare un documento, una versione di un documento, una cartella, una raccolta documenti, un elenco, un'app, un sito o una raccolta siti. Di seguito sono riportati alcuni esempi dei messaggi di errore che possono essere ricevuti se si tenta di eliminare un elemento che viene conservato:

- "Questo sito non può essere eliminato perché è incluso in un criterio di conservazione o blocco di eDiscovery"
- "Questo sito ha un criterio di conformità impostato per bloccare l'eliminazione"
- "Un criterio di conformità sta attualmente bloccando l'eliminazione di questo sito"
- "Questa raccolta siti non può essere eliminata perché contiene siti inclusi in un criterio di conservazione o blocco di eDiscovery"
- "È necessario eliminare tutti gli elementi presenti in questa cartella prima di eliminare la cartella"
- "Le versioni di questo elemento non possono essere eliminate perché è in attesa o criteri di conservazione"
- "L'elemento non può essere eliminato mentre è in attesa"
- "L'etichetta applicata a questo elemento impedisce la modifica o l'eliminazione"
- "L'elenco non può essere eliminato durante il blocco o il criterio di conservazione"
- "L'elenco non può essere eliminato se è bloccato o se è stato applicato un criterio di conservazione"

Per eliminare gli elementi in uno di questi scenari, è necessario rimuovere il criterio di conservazione, l'etichetta di conservazione o il blocco eDiscovery (oppure è necessario escludere un sito da un criterio di conservazione). È necessario disabilitare o escludere il blocco corrispondente che causa questo problema. Dopo la rimozione di un criterio di conservazione o di un blocco, potrebbero essere necessarie fino a 24 ore per rendere effettive le modifiche. 

Per informazioni sulle diverse funzionalità di conservazione e archiviazione che è possibile applicare a siti di SharePoint e account di OneDrive, vedere uno degli argomenti seguenti.

- [Panoramica dei criteri di conservazione](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)

- [Panoramica delle etichette di conservazione](https://docs.microsoft.com/microsoft-365/compliance/labels)

- [Gestione delle esenzioni in Advanced eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/managing-holds)

- [eDiscovery contiene](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-cases#step-4-place-content-locations-on-hold)

- [Criteri di eliminazione e chiusura dei siti legacy](https://support.office.com/article/Use-policies-for-site-closure-and-deletion-A8280D82-27FD-48C5-9ADF-8A5431208BA5)
