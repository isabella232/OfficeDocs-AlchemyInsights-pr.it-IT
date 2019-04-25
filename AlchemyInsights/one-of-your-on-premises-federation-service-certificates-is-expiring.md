---
title: Uno dei certificati del servizio federativo locale è in scadenza
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: e1afad0bab317af0f60a6ebda8c3ec8be398e38d
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32419696"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>Uno dei certificati del servizio federativo locale è in scadenza

Per risolvere il problema, attenersi alla seguente procedura:
  
- Installare il modulo di Microsoft Azure Active Directory per Windows PowerShell nel computer (se il modulo non è già installato). A tale scopo, accedere a [PowerShell di Azure Active Directory per il grafico](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- Seguire la procedura descritta nella sezione "scenario 1: il certificato per la firma di token AD FS scaduto" di ["si è verificato un problema durante l'accesso al sito" da ADFS quando un utente federato accede a Office 365, Azure o Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).
    
- Seguire i passaggi descritti in t[come aggiornare o ripristinare le impostazioni di un dominio federato in Office 365, Azure o Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
Per ulteriori informazioni sul rinnovo dei certificati di federazione, vedere [rinnovo del certificato per O365 e Azure ad](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
  

