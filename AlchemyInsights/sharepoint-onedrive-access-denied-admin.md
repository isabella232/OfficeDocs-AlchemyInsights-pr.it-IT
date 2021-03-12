---
title: Risoluzione dei problemi relativi ai messaggi di accesso negato
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3189fa61d28253569278024d4191ee63b917509f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707958"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Risolvere i problemi relativi ai messaggi di accesso negato nell'interfaccia di amministrazione di Sharepoint/OneDrive

Se si riceve un messaggio di accesso negato quando si tenta di passare a un'interfaccia di amministrazione di Sharepoint/OneDrive, assicurarsi di assegnare una licenza [all'utente.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users) Se l'utente ha una licenza, è inoltre necessario assicurarsi che gli sia assegnato un ruolo [di](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) amministratore in grado di accedere alle centri di amministrazione.

Questo problema può verificarsi anche quando un utente viene eliminato e ri creato di nuovo con lo stesso nome dell'entità utente (UPN). Il nuovo account viene creato utilizzando un valore PUID (ID univoco Passport) diverso. Quando l'utente tenta di accedere a una raccolta siti o a OneDrive, l'utente ha un PUID non corretto. Un secondo scenario prevede la sincronizzazione della directory con un'unità organizzativa (OU) di Active Directory. Se gli utenti hanno già eseguito l'accesso a SharePoint e quindi vengono spostati in un'unità organizzativa diversa e sincronizzati nuovamente con SharePoint, è possibile che si verifichi questo problema.

Per risolvere questo problema, è consigliabile ripristinare l'UPN originale con la procedura descritta nell'articolo Ripristinare [un utente in Microsoft 365.](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)

Nota: se un'interfaccia di amministrazione di OneDrive o SharePoint non è disponibile per più utenti che hanno avuto accesso in precedenza, potrebbe verificarsi un problema di servizio temporaneo.  [Controllare il dashboard sull'integrità del servizio.](https://portal.office.com/adminportal/home#/servicehealth)


