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
ms.openlocfilehash: 3f1f9728cdcfbe5676e5afc45b2afe82836fed9c8907df3559ac7daec21194ed
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54090416"
---
# <a name="configure-ldap"></a>Configurare LDAP

Per configurare LDAP, eseguire le operazioni seguenti:

1. Controllare l'integrità del dominio nel [portale di Azure.](https://aka.ms/aadds-health)
1. Verificare che sia disponibile una sottoscrizione di Azure AD valida e che Servizi di dominio Azure AD sia stato abilitato.
1. Il certificato necessario per abilitare LDAP sicuro deve essere ottenuto da un'autorità di certificazione pubblica attendibile o essere un certificato autofirmato.
1. Verificare che il certificato segua le linee guida [necessarie.](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate)

**Certificato non valido**
1. Per rinnovare un certificato, seguire la procedura per creare un nuovo certificato e ricaricarlo: [Configurare LDAP.](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)
1. Per risolvere il problema noto con avvisi LDAP protetti in Servizi di dominio Azure Active Directory, vedere [Risolvere gli avvisi LDAP.](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)
