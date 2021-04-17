---
title: Non è possibile accedere all'interfaccia di amministrazione di SharePoint o OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001459"
- "5638"
ms.openlocfilehash: 7ba4a9c6995c03dd21e0e1aa387e407d41a08fb1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824439"
---
# <a name="unable-to-access-sharepoint-or-onedrive-admin-center"></a>Non è possibile accedere all'interfaccia di amministrazione di SharePoint o OneDrive

- Se il sito dell'interfaccia di amministrazione di SharePoint o OneDrive non è accessibile o disponibile, è possibile che si sia verificato un problema temporaneo per cui gli utenti riscontrano ritardi intermittenti o errori di navigazione durante l'accesso ai siti di SharePoint o ai contenuti di OneDrive. Controllare il [dashboard sull'integrità dei servizi](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) per verificare se l'organizzazione è interessata.

- Agli amministratori globali e di SharePoint è necessario assegnare una licenza di SharePoint. Gli account appena creati ai quali è stata appena assegnata una licenza o un ruolo di amministratore di SharePoint potrebbero riscontrare problemi di accesso a SharePoint, ad esempio di tipo "accesso negato" o "utente non trovato". Attendere almeno 24 ore per il completamento della sincronizzazione tra i sistemi. Ci rendiamo conto che 24 ore può sembrare molto. In molti casi, stiamo già lavorando a una soluzione.

- Gli utenti di Privileged Identity Management ([PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new)) potrebbero ricevere un messaggio di accesso negato se la finestra di tempo di accesso consentito è molto piccola, vedere [Accesso negato agli account PIM](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts).