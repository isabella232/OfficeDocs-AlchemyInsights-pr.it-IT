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
# <a name="configure-ldap"></a><span data-ttu-id="5e5d6-102">Configurare LDAP</span><span class="sxs-lookup"><span data-stu-id="5e5d6-102">Configure LDAP</span></span>

<span data-ttu-id="5e5d6-103">Per configurare LDAP, eseguire le operazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="5e5d6-103">To configure LDAP, do the following:</span></span>

1. <span data-ttu-id="5e5d6-104">Controllare l'integrità del dominio sul [portale di Azure](https://aka.ms/aadds-health).</span><span class="sxs-lookup"><span data-stu-id="5e5d6-104">Check your domain’s health on the [Azure portal](https://aka.ms/aadds-health).</span></span>
1. <span data-ttu-id="5e5d6-105">Verificare che sia disponibile una sottoscrizione di Azure AD valida e che i servizi di dominio di Azure AD siano stati abilitati.</span><span class="sxs-lookup"><span data-stu-id="5e5d6-105">Ensure a valid Azure AD subscription is available and Azure AD Domain Services has been enabled.</span></span>
1. <span data-ttu-id="5e5d6-106">Il certificato richiesto per abilitare il protocollo LDAP sicuro deve essere ottenuto da un'autorità di certificazione pubblica attendibile o da un certificato autofirmato.</span><span class="sxs-lookup"><span data-stu-id="5e5d6-106">The certificate required to enable secure LDAP must be obtained from a trusted public certification authority or be a self-signed certificate.</span></span>
1. <span data-ttu-id="5e5d6-107">Verificare che il certificato segua le [linee guida](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate)necessarie.</span><span class="sxs-lookup"><span data-stu-id="5e5d6-107">Ensure the certificate follows the required [guidelines](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).</span></span>

<span data-ttu-id="5e5d6-108">**Certificato non valido**</span><span class="sxs-lookup"><span data-stu-id="5e5d6-108">**Invalid Certificate**</span></span>
1. <span data-ttu-id="5e5d6-109">Per rinnovare un certificato, eseguire la procedura seguente per creare un nuovo certificato e ricaricare: [Configure LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="5e5d6-109">To renew a certificate, follow the steps to create a new certificate and reupload: [Configure LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
1. <span data-ttu-id="5e5d6-110">Per risolvere i problemi noti con gli avvisi LDAP sicuri in servizi di dominio Active Directory di Azure, vedere [risolvere gli avvisi LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="5e5d6-110">To resolve known issue with Secure LDAP alerts in Azure Active directory Domain Services, see [Resolve LDAP alerts](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
