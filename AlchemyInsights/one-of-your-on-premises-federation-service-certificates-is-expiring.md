---
title: Uno dei certificati del servizio federativo locale scade
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: d0658b05b81ac45e7ce80323ad29898599482c4d3430d886627af6e9f8d136f6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53985221"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>Uno dei certificati del servizio federativo locale scade

Per risolvere il problema, attenersi alla seguente procedura:
  
- Installare il Microsoft Azure Active Directory per Windows PowerShell nel computer (se il modulo non è già installato). A tale scopo, passare [a Azure Active Directory PowerShell per Graph](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- Seguire i passaggi descritti nella sezione "Scenario 1: Il certificato di firma token AD FS è scaduto" dell'errore "Si è verificato un problema di accesso al sito" da AD FS quando un utente federato accede [a Microsoft 365, Azure o Intune.](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)
    
- Seguire i passaggi descritti in Come aggiornare o ripristinare le impostazioni di un dominio [federato in Microsoft 365, Azure o Intune.](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)
    
Per ulteriori informazioni sul rinnovo dei certificati federativi, vedere [Rinnovo dei certificati per O365 e Azure AD.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)
  

