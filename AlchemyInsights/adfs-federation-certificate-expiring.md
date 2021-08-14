---
title: Scadenza del certificato di federazione ADFS
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
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 48d4ccbbc0ed3dc54cbcd17ae7b9040bfd9ecc426897c06b653bf40bc7d5e9b2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53952973"
---
# <a name="adfs-federation-certificate-expiring"></a>Scadenza del certificato di federazione ADFS

Per risolvere il problema, attenersi alla seguente procedura:
  
1. Installare il Microsoft Azure Active Directory per Windows PowerShell nel computer (se il modulo non è già installato). A tale scopo, passare a [Gestire Azure AD usando Windows PowerShell](https://aka.ms/aadposh).

2. Seguire i passaggi descritti nella sezione "Scenario 1: Il certificato di firma token AD FS è scaduto" dell'errore "Si è verificato un problema di accesso al sito" da AD FS quando un utente federato accede [a Microsoft 365, Azure o Intune.](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)

3. Seguire i passaggi descritti in [Aggiornare o ripristinare le impostazioni di un dominio federato in Microsoft, Azure o Intune.](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)

    Per ulteriori informazioni sul rinnovo dei certificati federativi, vedere [Renew federation certificates for Microsoft 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
