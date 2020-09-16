---
title: Non è possibile accedere all'interfaccia di amministrazione di SharePoint o OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001459"
- "5638"
ms.openlocfilehash: a70b0708b325c5feaefec3d97c957086d7f62cc6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749482"
---
# <a name="unable-to-access-sharepoint-or-onedrive-admin-center"></a>Non è possibile accedere all'interfaccia di amministrazione di SharePoint o OneDrive

- Se il sito dell'interfaccia di amministrazione di SharePoint o OneDrive non è accessibile o disponibile, è possibile che si sia verificato un problema temporaneo per cui gli utenti riscontrano ritardi intermittenti o errori di navigazione durante l'accesso ai siti di SharePoint o ai contenuti di OneDrive. Controllare il [dashboard sull'integrità dei servizi](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) per verificare se l'organizzazione è interessata.

- Agli amministratori globali e di SharePoint è necessario assegnare una licenza di SharePoint. Gli account appena creati ai quali è stata appena assegnata una licenza o un ruolo di amministratore di SharePoint potrebbero riscontrare problemi di accesso a SharePoint, ad esempio di tipo "accesso negato" o "utente non trovato". Attendere almeno 24 ore per il completamento della sincronizzazione tra i sistemi. Ci rendiamo conto che 24 ore può sembrare molto. In molti casi, stiamo già lavorando a una soluzione.

- Gli utenti di Privileged Identity Management ([PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new)) potrebbero ricevere un messaggio di accesso negato se la finestra di tempo di accesso consentito è molto piccola, vedere [Accesso negato agli account PIM](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts).