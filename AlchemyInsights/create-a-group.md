---
title: Creare un gruppo
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
- "9003234"
- "7230"
ms.openlocfilehash: 4530abb3bf597458ea22441203a0db24b4b109f0760258310072891014c4b454
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929309"
---
# <a name="create-a-group"></a>Creare un gruppo

In questo argomento viene descritta la creazione di gruppi.

**Autorizzazione per la creazione di un gruppo**

Assicurarsi di essere autorizzati a creare un nuovo gruppo. Gli amministratori globali possono disabilitare la creazione di gruppi nel portale di Azure o nel riquadro di accesso. Potrebbe essere necessario un amministratore per creare il nuovo gruppo o per farsi assegnare le autorizzazioni appropriate.

**Gestire le autorizzazioni per la creazione di gruppi**

1. Gli amministratori globali possono gestire le autorizzazioni per la creazione di gruppi (per motivi di sicurezza) o i gruppi di Office 365 creati nel portale di Azure o nel pannello di accesso, scegliendo "Gli utenti possono creare gruppi di sicurezza nei portali di Azure" o "Gli utenti possono creare gruppi di Office 365 nei portali di Azure" **in** Tutti i gruppi Generale  >  **(Impostazioni).**
2. È inoltre possibile limitare la creazione di gruppi per selezionare un gruppo di utenti se si dispone di una licenza Azure Active Directory P1 Premium licenza.

**Disabilitazione della notifica di benvenuto per i nuovi Office 365 membri del gruppo**

La notifica di benvenuto inviata agli utenti aggiunti Office 365 gruppi può essere disabilitata impostando **UnifiedGroupWelcomeMessageEnabled** su False in PowerShell. Altre informazioni su questa impostazione [qui](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).

