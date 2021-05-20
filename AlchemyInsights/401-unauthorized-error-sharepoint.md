---
title: Errore 401 Non autorizzato in SharePoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10935"
- "9001435"
ms.openlocfilehash: ac2fe27a8e7b277bfaf18303bf5b792410a1ea6a
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539936"
---
# <a name="401-unauthorized-error-in-sharepoint"></a>Errore 401 Non autorizzato in SharePoint

Se viene visualizzato l'errore "(401) Non autorizzato" in SharePoint, tale problema potrebbe essere correlato alla deprecazione di TLS 1.0/1.1. Per altre informazioni, vedere:

- [Preparazione per TLS 1.2 in Office 365 e Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Si verificano errori di autenticazione se il client non dispone del supporto TLS 1.2](/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Aggiornamento per abilitare TLS 1.1 e TLS 1.2 come protocolli sicuri predefiniti in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Se gli utenti hanno Windows 7, verificare che selezionino i [pacchetti di crittografia TLS in Windows 7](/windows/win32/secauthn/tls-cipher-suites-in-windows-7).