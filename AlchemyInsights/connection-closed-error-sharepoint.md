---
title: Errore di chiusura della connessione sottostante in SharePoint
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 04/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10802"
- "9006390"
ms.openlocfilehash: 1b4f336f389eb6fd81ac2ca40e6047184cc4c1bf
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58317700"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a>Errore "La connessione sottostante è stata chiusa" in SharePoint

Se viene visualizzato l'errore "La connessione sottostante è stata chiusa" in SharePoint, tale problema potrebbe essere legato alla deprecazione di TLS 1.0/1.1. Per altre informazioni vedere questi articoli:

- [Preparazione per TLS 1.2 in Office 365 e Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Si verificano errori di autenticazione se il client non dispone del supporto TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Aggiornamento per abilitare TLS 1.1 e TLS 1.2 come protocolli sicuri predefiniti in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Se gli utenti hanno Windows 7, verificare che selezionino i [pacchetti di crittografia TLS in Windows 7](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7).