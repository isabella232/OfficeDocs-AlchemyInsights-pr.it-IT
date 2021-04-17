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
ms.openlocfilehash: 3ba6e6a6f93225bc843dfd1a028d31223f01280c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821955"
---
# <a name="adfs-federation-certificate-expiring"></a>Scadenza del certificato di federazione ADFS

Per risolvere il problema, attenersi alla seguente procedura:
  
1. Installare il modulo di Microsoft Azure Active Directory Windows PowerShell nel computer (se il modulo non è già installato). A tale scopo, passare a [Gestire Azure AD usando Windows PowerShell](https://aka.ms/aadposh).

2. Seguire i passaggi descritti nella sezione "Scenario 1: Il certificato di firma token AD FS è scaduto" dell'errore "Si è verificato un problema di accesso al sito" da AD FS quando un utente federato accede [a Microsoft 365, Azure o Intune.](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)

3. Seguire i passaggi descritti in [Aggiornare o ripristinare le impostazioni di un dominio federato in Microsoft, Azure o Intune.](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)

    Per ulteriori informazioni sul rinnovo dei certificati federativi, vedere Rinnovare i certificati [di federazione per Microsoft 365 e Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)
