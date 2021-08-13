---
title: Risoluzione dei problemi di accesso ai messaggi negati OneDrive for Business siti
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
ms.openlocfilehash: fc4a2bd7dcc74f5f05e8b709e4bc3eac6ed445d6e2ea9ede698abbc8667723ce
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957797"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Risoluzione dei problemi di accesso ai messaggi negati OneDrive for Business siti

Questo problema si verifica più frequentemente quando un utente viene eliminato e ri-creato con lo stesso nome dell'entità utente (UPN). Il nuovo account viene creato utilizzando un valore PUID (ID univoco Passport) diverso. Quando l'utente tenta di accedere a una raccolta siti o al OneDrive, l'utente ha un PUID non corretto. Un secondo scenario prevede la sincronizzazione della directory con un'unità organizzativa (OU) di Active Directory. Se gli utenti hanno già eseguito l'accesso a SharePoint e quindi vengono spostati in un'altra unità organizzativa e sincronizzati nuovamente con SharePoint, è possibile che si verifichi questo problema.

1. Per risolvere questo problema, è necessario ripristinare l'UPN originale con i passaggi descritti nell'articolo, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).
2. Se non è possibile ripristinare l'utente originale, è consigliabile rimuovere l'utente precedente dal sito di OneDrive usando questa procedura, Rimuovere un utente [dall'elenco delle informazioni utente.]() 
3. Al termine di questa operazione, è possibile verificare che l'utente abbia diritti di amministratore per il sito di OneDrive seguendo la procedura per Aggiungere [l'amministratore](https://docs.microsoft.com/sharepoint/manage-user-profiles) per il sito di un OneDrive

Per ulteriori informazioni sui livelli di autorizzazione, vedere l'articolo [Informazioni sui livelli di autorizzazione in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
