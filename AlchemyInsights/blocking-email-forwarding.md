---
title: 726 blocco dell'inoltro della posta elettronica
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: c0d9ed14f83d3c7d47e1728d5ed9ca3a19412ad2
ms.sourcegitcommit: f74c9698a31634154ce58dda8b3145bb10685ace
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/23/2020
ms.locfileid: "48219859"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Blocco o sblocco dell'inoltro della posta elettronica

Per abilitare o disabilitare l'inoltro della posta elettronica per una cassetta postale specifica, vedere [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

A livello di tenant, il controllo dell'inoltro esterno viene effettuato utilizzando il criterio di protezione dalla posta indesiderata in uscita. Se è impostato su disattivato o automatico, potrebbe bloccare l'inoltro della posta elettronica con il messaggio di errore "550 5.7.520 Access Denied, l'organizzazione non consente l'inoltro esterno". Successivamente, se l'inoltro è stato impostato per essere bloccato, questo è l'errore che vedranno gli utenti.

Se l'inoltro viene bloccato, verificare che i criteri siano configurati per abilitare l'inoltro AutoForward esterno. È possibile controllare il criterio del filtro della posta indesiderata in uscita dal centro sicurezza e conformità o eseguendo il comando Get-HostedOutboundSpamFilterPolicy | nome FL, AutoForwardingMode. Se si desidera configurare il blocco AutoForward, lo stesso comando diranno lo stato dei criteri ora.

Nota: si consiglia di mantenere disattivata l'AutoForward esterno sui criteri di filtro della posta indesiderata in uscita predefiniti e di abilitarla solo per gli utenti che hanno bisogno di un inoltro esterno creando un criterio personalizzato per tali utenti. Per ulteriori informazioni, vedere [configurazione dell'inoltro della posta elettronica esterno in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).