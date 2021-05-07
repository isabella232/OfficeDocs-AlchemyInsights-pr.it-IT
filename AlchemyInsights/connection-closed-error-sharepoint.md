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
ms.openlocfilehash: b64215b5b83ef1092eb58791e6dbb015b72d422d
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233430"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a>Errore "La connessione sottostante è stata chiusa" in SharePoint

Se viene visualizzato l'errore "La connessione sottostante è stata chiusa" in SharePoint, tale problema potrebbe essere legato alla deprecazione di TLS 1.0/1.1. Per altre informazioni vedere questi articoli:

- [Preparazione per TLS 1.2 in Office 365 e Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide)

- [Si verificano errori di autenticazione se il client non dispone del supporto TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

Se gli utenti hanno Windows 7, verificare che selezionino i [pacchetti di crittografia TLS in Windows 7](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7).