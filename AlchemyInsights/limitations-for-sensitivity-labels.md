---
title: Limitazioni per le etichette di riservatezza per i file di Office in SharePoint e OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12451"
- "9000181"
ms.openlocfilehash: c3a0695dc2aa5f6e56be2235f08c81dbbe7fcea2
ms.sourcegitcommit: 86c95d3f0f268e500b3732243ca85a650b2e7b8f
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 07/22/2021
ms.locfileid: "53533000"
---
# <a name="limitations-for-sensitivity-labels-for-office-files-in-sharepoint-and-onedrive"></a>Limitazioni per le etichette di riservatezza per i file di Office in SharePoint e OneDrive

Quando si abilitano le etichette di riservatezza per i file di Office in SharePoint e OneDrive, tenere presenti i requisiti e le limitazioni, tra cui:

- SharePoint e OneDrive non possono elaborare alcuni file etichettati e crittografati dalle app desktop di Office quando i file contengono dati di PowerQuery, dati archiviati da componenti aggiuntivi personalizzati o parti XML personalizzate.
- SharePoint e OneDrive non applicano automaticamente le etichette di riservatezza ai file esistenti già crittografati usando etichette di Azure Information Protection (AIP). Per applicare le etichette di riservatezza ai file crittografati: 
    - Assicurarsi che le etichette AIP siano state migrate e pubblicate nel Centro conformità Microsoft 365.
    - Scaricare i file etichettati, quindi caricarli nel percorso originale di SharePoint o OneDrive.
- Per i documenti crittografati, la stampa non è supportata.

Per altre informazioni sulle limitazioni, vedere [Abilitare le etichette di riservatezza per i file di Office in SharePoint e OneDrive](/microsoft-365/compliance/sensitivity-labels-sharepoint-onedrive-files#limitations).
