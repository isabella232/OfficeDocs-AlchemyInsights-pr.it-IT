---
title: "Risolvere i problemi relativi all'accesso Single #A0 per i dispositivi aggiunti ad Azure AD"
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "9327"
ms.openlocfilehash: d11c24719eb2db9e9fd87c158c80cec5cb75b946
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/19/2021
ms.locfileid: "50898083"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a>Risolvere i problemi relativi all'accesso Single #A0 per i dispositivi aggiunti ad Azure AD

Se si dispone di un ambiente Active Directory (AD) locale e si desidera aggiungere i computer aggiunti al dominio DI AD ad Azure AD, è possibile eseguire questa operazione eseguendo l'aggiunta ibrida di Azure AD. [Procedura: Pianificare l'implementazione ibrida](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) dell'aggiunta ad Azure Active Directory fornisce i passaggi correlati per implementare un'aggiunta ibrida di Azure AD nell'ambiente.

Per ulteriori informazioni, vedere [Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).

**Problemi relativi al token di aggiornamento primario**

Un token di aggiornamento primario (PRT) è un elemento chiave dell'autenticazione di Azure AD nei dispositivi Windows 10, Windows Server 2016 e versioni successive, iOS e Android. Si tratta di un token Web JSON (JWT) rilasciato appositamente ai broker di token di prima parte Microsoft per abilitare single sign-on (SSO) tra le applicazioni usate in tali dispositivi. Per informazioni dettagliate su come viene emesso, usato e protetto un PRT nei dispositivi Windows 10, vedi Che [cos'è un token di aggiornamento primario?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

**WamDefaultSet: SÌ e AzureADPrt: SÌ**

Questi campi indicano se l'utente ha eseguito correttamente l'autenticazione in Azure AD durante l'accesso al dispositivo. Se i valori sono **NO**, potrebbe essere dovuto a:

- Chiave di archiviazione non compatibile nel TPM associato al dispositivo al momento della registrazione (controllare KeySignTest durante l'esecuzione con privilegi elevati)
- ID di accesso alternativo
- Proxy HTTP non trovato

Per risolvere i problemi relativi ai dispositivi tramite il comando dsregcmd, vedere [Stato SSO.](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
