---
title: Messaggi di posta elettronica mancanti in quarantena
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: c77da6716c0755d6ed4911f490e000bd74d08f92
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329666"
---
# <a name="missing-emails-in-quarantine"></a>Messaggi di posta elettronica mancanti in quarantena

Gli amministratori [possono visualizzare, rilasciare o eliminare questi messaggi](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

Nel portale Microsoft 365 Defender, <https://security.microsoft.com> passare a **Revisione** \> **quarantena**. In caso contrario, per passare direttamente alla **pagina Quarantena,** utilizzare <https://security.microsoft.com/quarantine> .  

Per ulteriori informazioni sui valori di ricerca/filtro che è possibile utilizzare, vedere [Manage quarantined messages and files as an admin in EOP.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

I cmdlet utilizzati per visualizzare e gestire i messaggi e i file in quarantena sono:

- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): questo cmdlet è valido solo per i messaggi e non per i file Cassaforte Allegati per SharePoint, OneDrive o Microsoft Teams.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)
