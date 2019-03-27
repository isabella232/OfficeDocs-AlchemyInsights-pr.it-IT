---
title: Risoluzione dei problemi relativi alla sincronizzazione delle password
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
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 1320c0fe839337188162824439be6f15f86b6c90
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/22/2019
ms.locfileid: "30767180"
---
# <a name="troubleshoot-password-synchronization"></a>Risoluzione dei problemi relativi alla sincronizzazione delle password

Per risolvere i problemi in cui nessuna password è sincronizzata con Azure AD Connect Version 1.1.614.0 o versione successiva:
  
1. Aprire una nuova sessione di Windows PowerShell nel server Azure AD Connect con l'opzione **Esegui come amministratore** . 
    
2. Eseguire **Set-ExecutionPolicy RemoteSigned** o **Set-ExecutionPolicy**Unrestricted. 
    
3. Avviare la procedura guidata di Azure AD Connect.
    
4. Passare alla pagina * * attività aggiuntive * *, selezionare * * risoluzione dei problemi * * e fare clic su **Avanti**. 
    
5. Nella pagina risoluzione dei problemi fare clic su **Avvia per avviare il menu Risoluzione dei problemi** in PowerShell. 
    
6. Nel menu principale, selezionare **risoluzione dei problemi relativi alla sincronizzazione delle password**. 
    
7. Nel menu secondario selezionare **sincronizzazione password non funziona affatto**. 
    
 **Informazioni sui risultati dell'attività di risoluzione dei problemi**
  
L'attività di risoluzione dei problemi esegue i controlli seguenti:
  
- Verifica che la funzionalità di sincronizzazione delle password sia abilitata per il tenant di Azure AD.
    
- Verifica che il server Azure AD Connect non sia in modalità di gestione temporanea.
    
- Per ogni connettore Active Directory locale esistente (che corrisponde a una foresta di Active Directory esistente):
    
- 
  - Verifica che la funzionalità di sincronizzazione delle password sia abilitata.
    
  - Cerca gli eventi heartbeat di sincronizzazione delle password nei registri eventi applicazioni di Windows.
    
  - Per ogni dominio di Active Directory sotto il connettore Active Directory locale:
    
  - Verifica che il dominio sia raggiungibile dal server Azure AD Connect.
    
  - Verifica che gli account di servizi di dominio Active Directory utilizzati dal connettore Active Directory locale dispongano del nome utente, della password e delle autorizzazioni corretti necessari per la sincronizzazione delle password.
    
Per ulteriori informazioni sulla risoluzione dei problemi relativi alla sincronizzazione delle password, vedere [risolvere i problemi di sincronizzazione delle password con Azure ad Connect Sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).
  

