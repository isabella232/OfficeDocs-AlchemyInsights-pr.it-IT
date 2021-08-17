---
title: 726 Blocking email forwarding
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
ms.openlocfilehash: 0bff7ede02809e133dc6616452ec840f552bd4fa6c45b7987d6455b2a9ba49bf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059636"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Blocco o sblocco dell'inoltro della posta elettronica

Per abilitare o disabilitare l'inoltro della posta elettronica per una cassetta postale specifica, vedere [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

A livello di tenant, il controllo dell'inoltro esterno viene eseguito utilizzando i criteri di posta indesiderata in uscita. È possibile controllare i criteri di filtro [](https://protection.office.com/antispam) della posta indesiderata in uscita dal Centro sicurezza e conformità qui o utilizzando il [comando Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).

Se viene visualizzato l'errore seguente: **"550 5.7.520** Accesso negato, l'organizzazione non consente l'inoltro esterno", assicurarsi che il criterio sia configurato per abilitare l'inoltro automatico esterno.

**Nota:** È consigliabile mantenere il criterio di filtro della posta indesiderata esterno disabilitato nel criterio di filtro della posta indesiderata in uscita predefinito e abilitarlo solo per gli utenti che necessitano dell'inoltro esterno creando un criterio personalizzato per tali utenti. Per ulteriori informazioni, vedere [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).