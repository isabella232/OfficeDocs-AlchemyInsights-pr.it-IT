---
title: Risoluzione dei problemi relativi ai messaggi di accesso negato ai siti di OneDrive for business
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9001cf0b7d9f1f05a2ecedca2c3137dd1b8a1c38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670620"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Risoluzione dei problemi relativi ai messaggi di accesso negato ai siti di OneDrive for business

Questo problema si verifica più frequentemente quando un utente viene eliminato e ricreato con lo stesso nome dell'entità utente (UPN, User Principal Name). Il nuovo account viene creato utilizzando un valore PUID (Passport Unique ID) diverso. Quando l'utente tenta di accedere a una raccolta siti o ai propri OneDrive, l'utente ha un PUID non corretto. Un secondo scenario implica la sincronizzazione della directory con un'unità organizzativa di Active Directory. Se gli utenti hanno già effettuato l'accesso a SharePoint e quindi vengono spostati in un'altra unità organizzativa e risincronizzati con SharePoint, potrebbero verificarsi questo problema.

1. Per risolvere il problema, è necessario ripristinare l'UPN originale con i passaggi descritti nell'articolo, [ripristinare un utente in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).
2. Se non è possibile ripristinare l'utente originale, è necessario rimuovere l'utente precedente dal sito di OneDrive utilizzando questi passaggi, [rimuovere un utente dall'elenco informazioni utente](). 
3. Una volta completata questa operazione, è possibile verificare che l'utente disponga dei diritti di amministratore per il sito di OneDrive attenendosi alla procedura seguente per [aggiungere l'amministratore per l'OneDrive di un utente](https://docs.microsoft.com/sharepoint/manage-user-profiles) .

Per ulteriori informazioni sui livelli di autorizzazione, vedere l'articolo, informazioni sui [livelli di autorizzazione in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
