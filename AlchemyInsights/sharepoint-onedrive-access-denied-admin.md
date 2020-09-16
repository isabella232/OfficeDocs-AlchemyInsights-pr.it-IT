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
ms.openlocfilehash: 22f5966fdae563c44affb7d0447787a4ee0aca93
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767666"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Risoluzione dei problemi relativi ai messaggi di accesso negato nell'interfaccia di amministrazione di SharePoint/OneDrive

Se si riceve un messaggio di accesso negato quando si tenta di accedere a un interfaccia di amministrazione di SharePoint/OneDrive, assicurarsi [di assegnare una licenza all'utente](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). Se l'utente dispone di una licenza, è necessario assicurarsi che sia [assegnato un ruolo di amministratore](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) che può accedere ai centri di amministrazione.

Questo problema può verificarsi anche quando un utente viene eliminato e ricreato con lo stesso nome dell'entità utente (UPN). Il nuovo account viene creato utilizzando un valore PUID (Passport Unique ID) diverso. Quando l'utente tenta di accedere a una raccolta siti o ai propri OneDrive, l'utente ha un PUID non corretto. Un secondo scenario implica la sincronizzazione della directory con un'unità organizzativa di Active Directory. Se gli utenti hanno già effettuato l'accesso a SharePoint e quindi vengono spostati in un'altra unità organizzativa e risincronizzati con SharePoint, potrebbero verificarsi questo problema.

Per risolvere il problema, è necessario ripristinare l'UPN originale con i passaggi descritti nell'articolo, [ripristinare un utente in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).

Nota: se un'interfaccia di amministrazione di OneDrive o SharePoint non è disponibile per più utenti che in precedenza avevano accesso, potrebbe verificarsi un problema di servizio temporaneo.  [Controllare il dashboard dell'integrità dei servizi](https://portal.office.com/adminportal/home#/servicehealth).


