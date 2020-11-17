---
title: Creare un gruppo
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086391"
---
# <a name="create-a-group"></a>Creare un gruppo

In questo argomento viene descritta la creazione di gruppi.

**Autorizzazione per la creazione di un gruppo**

Assicurarsi di essere autorizzati a creare un nuovo gruppo. Gli amministratori globali possono disabilitare la creazione del gruppo nel portale di Azure o nel pannello di accesso. Potrebbe essere necessario un amministratore per creare il nuovo gruppo o per fornire le autorizzazioni appropriate.

**Gestire le autorizzazioni per la creazione di gruppi**

1. Gli amministratori globali possono gestire le autorizzazioni per la creazione di gruppi (per motivi relativi alla sicurezza) o i gruppi di Office 365 creati nel portale di Azure o nel pannello di accesso, scegliendo "gli utenti possono creare gruppi di sicurezza nei portali di Azure" o "gli utenti possono creare gruppi di Office 365 nei portali di Azure" in **tutti i gruppi**  >  **generale (impostazioni)**.
2. È inoltre possibile limitare la creazione di gruppi per selezionare un gruppo di utenti se si dispone di una licenza di Azure Active Directory P1 Premium.

**Disabilitazione della notifica di benvenuto per i nuovi membri del gruppo di Office 365**

La notifica di benvenuto inviata agli utenti che sono stati aggiunti ai gruppi di Office 365 può essere disattivata impostando **UnifiedGroupWelcomeMessageEnabled** su false in PowerShell. Per ulteriori informazioni su [questa impostazione,](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)vedere.

