---
title: Bloccare o sbloccare l'inoltro automatico esterno della posta elettronica
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
ms.openlocfilehash: fe9e52023b809b38c43332a10a1184d114798cfe
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58315878"
---
# <a name="block-or-unblock-eternal-automatic-email-forwarding"></a>Bloccare o sbloccare l'inoltro automatico della posta elettronica

Per abilitare o disabilitare l'inoltro della posta elettronica per una cassetta postale specifica, vedere [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

Gli amministratori possono controllare l'inoltro esterno per l'organizzazione utilizzando i [criteri di posta indesiderata in uscita.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy) È possibile gestire i criteri di posta indesiderata in uscita nel portale Microsoft 365 Defender o utilizzando il <https://security.microsoft.com/antispam> cmdlet [Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy) in Exchange Online PowerShell.

Se viene visualizzato il seguente errore: **"550 5.7.520** Accesso negato, l'organizzazione non consente l'inoltro esterno", verificare che il criterio sia configurato per abilitare i messaggi inoltrati automaticamente esterni.

**Nota:** è consigliabile il valore predefinito  **Automatico -** Sistema controllato per l'impostazione Regole di inoltro automatico nel criterio di filtro della posta indesiderata in uscita predefinito (l'inoltro esterno automatico è bloccato; l'inoltro automatico interno funziona ancora). È consigliabile creare criteri di filtro della posta indesiderata in uscita personalizzati e utilizzare il valore **Attivato -** L'inoltro è abilitato solo per gli utenti che necessitano dell'inoltro automatico esterno della posta elettronica. Per ulteriori informazioni, vedere [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).
