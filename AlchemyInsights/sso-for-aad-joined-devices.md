---
title: Single-Sign per i dispositivi Azure Active Directory aggiunti
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9891"
ms.openlocfilehash: 365225926296677feb7853481651a634792fd8bfa9abd9dc9359ffaae50b60eb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050014"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a>Single #A0 per Azure Active Directory aggiunti

Se si dispone di un ambiente Active Directory (AD) locale e si desidera aggiungere i computer aggiunti al dominio DI AD ad Azure AD, è possibile eseguire questa operazione eseguendo l'aggiunta ibrida di Azure AD. [Procedura: Pianificare l'implementazione](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) Azure Active Directory join ibrido fornisce i passaggi correlati per implementare un'aggiunta ibrida di Azure AD nell'ambiente.

[Configurare i dispositivi aggiunti ad Azure AD per i dispositivi locali Single-Sign on using Windows Hello for Business](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

**Problemi relativi al token di aggiornamento primario** Un token di aggiornamento primario (PRT) è un elemento chiave dell'autenticazione di Azure AD nei dispositivi Windows 10, Windows Server 2016 e versioni successive, iOS e Android. Si tratta di un token Web JSON (JWT) rilasciato appositamente ai broker di token di prima parte Microsoft per abilitare single sign-on (SSO) tra le applicazioni usate in tali dispositivi. [In Che cos'è un token](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)di aggiornamento primario? verranno fornite informazioni dettagliate su come viene emesso, usato e protetto un PRT Windows 10 dispositivi.

**WamDefaultSet: SÌ e AzureADPrt: SÌ** Questi campi indicano se l'utente ha eseguito correttamente l'autenticazione in Azure AD durante l'accesso al dispositivo. Se i valori sono **NO,** potrebbe essere dovuto:

- Chiave di archiviazione non disponibile nel TPM associato al dispositivo al momento della registrazione (controllare KeySignTest durante l'esecuzione con privilegi elevati).
- ID di accesso alternativo
- Proxy HTTP non trovato

Risolvere i problemi relativi ai dispositivi tramite il comando dsregcmd - [Stato SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
