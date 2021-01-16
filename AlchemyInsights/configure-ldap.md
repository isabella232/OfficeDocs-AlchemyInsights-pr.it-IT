---
title: Configurare LDAP
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004394"
- "7923"
ms.openlocfilehash: b6e89bca4e924c5570123194cb26358ba2c162ce
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/15/2021
ms.locfileid: "49876572"
---
# <a name="configure-ldap"></a>Configurare LDAP

Per configurare LDAP, eseguire le operazioni seguenti:

1. Controllare l'integrità del dominio sul [portale di Azure](https://aka.ms/aadds-health).
1. Verificare che sia disponibile una sottoscrizione di Azure AD valida e che i servizi di dominio di Azure AD siano stati abilitati.
1. Il certificato richiesto per abilitare il protocollo LDAP sicuro deve essere ottenuto da un'autorità di certificazione pubblica attendibile o da un certificato autofirmato.
1. Verificare che il certificato segua le [linee guida](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate)necessarie.

**Certificato non valido**
1. Per rinnovare un certificato, eseguire la procedura seguente per creare un nuovo certificato e ricaricare: [Configure LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
1. Per risolvere i problemi noti con gli avvisi LDAP sicuri in servizi di dominio Active Directory di Azure, vedere [risolvere gli avvisi LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
