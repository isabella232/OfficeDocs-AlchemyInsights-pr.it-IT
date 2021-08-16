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
ms.openlocfilehash: 101c0ba90d2bec6b1684fd63645ba2f8f89783ad5bfdf0efe739d31dfd951f66
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044416"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a>Errore "La connessione sottostante è stata chiusa" in SharePoint

Se viene visualizzato l'errore "La connessione sottostante è stata chiusa" in SharePoint, tale problema potrebbe essere legato alla deprecazione di TLS 1.0/1.1. Per altre informazioni vedere questi articoli:

- [Preparazione per TLS 1.2 in Office 365 e Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Si verificano errori di autenticazione se il client non dispone del supporto TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Aggiornamento per abilitare TLS 1.1 e TLS 1.2 come protocolli sicuri predefiniti in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Se gli utenti hanno Windows 7, verificare che selezionino i [pacchetti di crittografia TLS in Windows 7](/windows/win32/secauthn/tls-cipher-suites-in-windows-7).