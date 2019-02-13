---
title: Federazione ADFS scadenza del certificato
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 55529265d2356a911624026107fb639f93e29abd
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29925384"
---
# <a name="adfs-federation-certificate-expiring"></a>Federazione ADFS scadenza del certificato

Per risolvere questo problema, eseguire la procedura seguente:
  
1. Installare il Microsoft Azure Active Directory Module per Windows PowerShell nel computer (se il modulo non è già installato). A tale scopo, passare a [Gestione Azure AD tramite Windows PowerShell](https://aka.ms/aadposh).
    
2. Seguire i passaggi descritti nel "Scenario 1: il certificato di firma di token ADFS scaduto" sezione di [errore "Problema durante l'accesso al sito" da ADFS quando un utente federato accede a Office 365, Azure o Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).
    
3. Seguire i passaggi della [procedura aggiornare o ripristinare le impostazioni di un dominio federato in Office 365, Azure o Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
    Per ulteriori informazioni su rinnovo di certificati di federazione, vedere [rinnovare i certificati di federazione per Office 365 e Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
    

