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
ms.openlocfilehash: c49dfbf422b312f4744711d5f12b0eb83b6ebf2e
ms.sourcegitcommit: b398afd92d4259f893c25b48aec65921e6cc68d6
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 05/16/2020
ms.locfileid: "44268776"
---
# <a name="teams-client-crashing"></a>Il client di Teams si arresta in modo anomalo?

Se il client di Teams si arresta in modo anomalo, provare le operazioni seguenti:

- Se si usa l'applicazione desktop di Teams, [verificare che l'app sia completamente aggiornata](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Assicurarsi che tutti gli [intervalli di indirizzi e gli URL di Microsoft 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) siano accessibili.

- Eseguire l'accesso con l'account amministratore del tenant e controllare il [Dashboard di integrità dei servizi](https://docs.microsoft.com/office365/enterprise/view-service-health) per verificare che non siano presenti interruzioni o riduzioni delle prestazioni del servizio.

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

Se il client di Teams si arresta ancora in modo anomalo, è possibile riprodurre il problema? In tal caso: 

1. Usare la Registrazione azioni utente per acquisire la procedura.
    - Chiudere TUTTE le applicazioni inutili o riservate.
    - Avviare la Registrazione azioni utente e riprodurre il problema durante l'accesso con l'account utente interessato.
    
2. Allegare il file al caso di supporto.
