---
title: Il client di Teams si arresta in modo anomalo?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ce37b260d126f876d2b6177515bd8a7c3874ef2c
ms.sourcegitcommit: d02e2b73aa7d0453d7baca1ea5a186cf6081d022
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 03/27/2020
ms.locfileid: "43030683"
---
# <a name="teams-client-crashing"></a>Il client di Teams si arresta in modo anomalo?

Se il client di Teams si arresta in modo anomalo, provare le operazioni seguenti:

- Se si usa l'applicazione desktop di Teams, [verificare che l'app sia completamente aggiornata](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Assicurarsi che tutti gli [intervalli di indirizzi e gli URL di Office 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) siano accessibili.

- Eseguire l'accesso con l'account amministratore e controllare la [Dashboard di integrità dei servizi](https://docs.microsoft.com/office365/enterprise/view-service-health) per verificare che non siano presenti interruzioni o riduzioni delle prestazioni del servizio.

 - Come ultimo passaggio, si può provare a cancellare la cache del client di Teams:

    1.  Chiudere il client desktop di Microsoft Teams. È possibile fare clic con il pulsante destro del mouse su **Teams** nell'area delle icone e fare clic su **Esci** o eseguire Gestione attività e arrestare completamente il processo.

    2.  Passare a Esplora file e digitare %appdata%\Microsoft\teams.

    3.  Una volta nella directory, vengono visualizzate alcune delle seguenti cartelle:

         - All'interno di **Application Cache**, passare a Cache ed eliminare gli eventuali file presenti nel percorso di Cache: %appdata%\Microsoft\teams\application cache\cache.

        - All'interno di **Blob_storage**, eliminare tutti i file: %appdata%\Microsoft\teams\blob_storage.

        - All'interno di **Cache**, eliminare tutti i file: %appdata%\Microsoft\teams\Cache.

        - All'interno di **databases**, eliminare tutti i file: %appdata%\Microsoft\teams\databases.

        - All'interno di **GPUCache**, eliminare tutti i file: %appdata%\Microsoft\teams\GPUcache.

        - All'interno di **IndexedDB**, eliminare tutti i file .db: %appdata%\Microsoft\teams\IndexedDB.

        - All'interno di **Local Storage**, eliminare tutti i file: %appdata%\Microsoft\teams\Local Storage.

        - Infine, all'interno di **tmp**, eliminare i file: %appdata%\Microsoft\teams\tmp.

    4. Riavviare il client di Teams.
