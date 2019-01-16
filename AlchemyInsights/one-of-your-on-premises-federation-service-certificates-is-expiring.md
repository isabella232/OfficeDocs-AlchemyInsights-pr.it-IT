---
title: Uno dei certificati locale Federation Service scada
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: 89a4dd910d43d70e849be19d5f88e281f6d19834
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/15/2019
ms.locfileid: "28295934"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>Uno dei certificati locale Federation Service scada

Per risolvere questo problema, eseguire la procedura seguente:
  
- Installare il Microsoft Azure Active Directory Module per Windows PowerShell nel computer (se il modulo non è già installato). A tale scopo, passare a [Azure Active Directory PowerShell di grafico](https://docs.microsoft.com/en-us/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- Seguire i passaggi descritti nel "Scenario 1: il certificato di firma di token ADFS scaduto" sezione di [errore "Problema durante l'accesso al sito" da ADFS quando un utente federato accede a Office 365, Azure o Intune](https://support.microsoft.com/en-us/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).
    
- Seguire i passaggi della[procedura aggiornare o ripristinare le impostazioni di un dominio federato in Office 365, Azure o Intune](https://support.microsoft.com/en-us/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)t.
    
Per ulteriori informazioni su rinnovo di certificati di federazione, vedere [il rinnovo dei certificati per Office 365 e Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
  

