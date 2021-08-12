---
title: Abilitare la sincronizzare dell'account personale di un utente con l'account aziendale in Microsoft Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9127"
- "9004429"
ms.openlocfilehash: 4c246fcc9ef0e3a79c3e68be491e3e7f5c6edb0b
ms.sourcegitcommit: e9fcd72e64d35f5ba14dfa0fbde39eae20d86cfe
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 07/27/2021
ms.locfileid: "53603281"
---
# <a name="enable-a-user-to-sync-a-personal-account-with-the-work-account-in-microsoft-edge"></a>Abilitare la sincronizzare dell'account personale di un utente con l'account aziendale in Microsoft Edge

Verificare che i criteri seguenti siano soddisfatti:

- Enterprise State Roaming abilitato nell'interfaccia di amministrazione di Azure Active Directory, con una sottoscrizione per Azure Active Directory Premium o Enterprise Mobility + Security (EMS). Per altre informazioni, vedere [Abilitare Enterprise State Roaming in Azure Active Directory](/azure/active-directory/devices/enterprise-state-roaming-enable).
- Verificare che siano soddisfatti uno o entrambi i criteri seguenti:
    - Il servizio Azure Information Protection abilitato per il tenant. Per informazioni dettagliate, vedere [Attivare la protezione di Azure Rights Management dall'interfaccia di amministrazione di Microsoft 365](/azure/information-protection/activate-office365).
    - La funzionalità Azure Active Directory Enterprise State Roaming (ESR) abilitata per qualsiasi utente o tenant. Per altre informazioni, vedere [Che cos'è l'Enterprise State Roaming?](/azure/active-directory/devices/enterprise-state-roaming-overview)

Se AIP ed ESR sono entrambi disabilitati, viene visualizzato un messaggio di errore che informa gli utenti che non è disponibile la sincronizzazione per gli account.