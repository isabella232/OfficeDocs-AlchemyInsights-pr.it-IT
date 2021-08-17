---
title: Sincronizzazione dell'hash delle password per il servizio di dominio
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 3c00105a67f70ae9ce11cd8bb922c4d84a320010d021414b9159948f7dc87dbc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54040870"
---
# <a name="password-hash-synchronization-for-domain-service"></a>Sincronizzazione dell'hash delle password per il servizio di dominio

**Se l'istanza di Azure AD DS chiede di abilitare la sincronizzazione hash della password**

Si verifica uno scenario in cui si esegue un ambiente ibrido con gli utenti che si sincronizzano da un ambiente locale di Servizi di dominio Azure Active Directory. Questo scenario si verifica nonostante la sincronizzazione hash delle password da Active Directory DS locale al tenant di Azure AD.

**Causa**

Questo problema si verifica perché Azure AD Connect per impostazione predefinita non sincronizza gli hash delle password legacy di New Technology LAN Manager (NTLM) e Kerberos necessari per Azure AD DS.

**Soluzione** 

È necessario configurare Azure AD Connect per sincronizzare gli hash delle password necessari per l'autenticazione NTLM e Kerberos.

Dopo la configurazione di Azure AD Connect, un evento di creazione di account o di modifica della password locale sincronizza anche gli hash delle password legacy con Azure AD. Vedere questa [per](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) altre informazioni e per indicazioni su come abilitare la sincronizzazione delle password negli ambienti ibridi di Azure AD DS.