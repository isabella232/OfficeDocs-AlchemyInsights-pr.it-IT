---
title: Risolvere i problemi relativi ai messaggi di accesso negato
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 9acde72f82a27c9f2faa2cf4d0417374aa5a294234da96080dc0498d07639248
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54085232"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Risolvere i problemi relativi ai messaggi di accesso negato in Sharepoint/OneDrive Admin Center

Se si riceve un messaggio di accesso negato quando si tenta di passare a un'interfaccia di amministrazione di Sharepoint/OneDrive, assicurarsi di assegnare una licenza [all'utente.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users) Se l'utente ha una licenza, è necessario assicurarsi che gli sia assegnato un ruolo [di](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) amministratore in grado di accedere alle interfaccia di amministrazione.

Questo problema può verificarsi anche quando un utente viene eliminato e ri-creato con lo stesso nome dell'entità utente (UPN). Il nuovo account viene creato utilizzando un valore PUID (ID univoco Passport) diverso. Quando l'utente tenta di accedere a una raccolta siti o al OneDrive, l'utente ha un PUID non corretto. Un secondo scenario prevede la sincronizzazione della directory con un'unità organizzativa (OU) di Active Directory. Se gli utenti hanno già eseguito l'accesso a SharePoint e quindi vengono spostati in un'altra unità organizzativa e sincronizzati nuovamente con SharePoint, è possibile che si verifichi questo problema.

Per risolvere questo problema, è necessario ripristinare l'UPN originale con i passaggi descritti nell'articolo Ripristinare un utente [in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).

Nota: se un OneDrive o SharePoint'interfaccia di amministrazione non è disponibile per più utenti che in precedenza avevano accesso, potrebbe verificarsi un problema temporaneo del servizio.  [Controllare il dashboard di integrità del servizio](https://portal.office.com/adminportal/home#/servicehealth).


