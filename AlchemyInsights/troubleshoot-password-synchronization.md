---
title: Risoluzione dei problemi di sincronizzazione delle password
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
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: c71fce8621057093d23891c26f7b0285fdc8b9ed
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/15/2019
ms.locfileid: "28296584"
---
# <a name="troubleshoot-password-synchronization"></a>Risoluzione dei problemi di sincronizzazione delle password

Per la risoluzione dei problemi in alcuna password non sono sincronizzati con Azure Active Directory Connect versione 1.1.614.0 o versione successiva:
  
1. Aprire una nuova sessione di Windows PowerShell nel server di Azure Active Directory Connetti con l'opzione **Esegui come amministratore** . 
    
2. Eseguire **Set-ExecutionPolicy RemoteSigned** o **Set-ExecutionPolicy Unrestricted**. 
    
3. Avviare la procedura guidata Connetti Azure Active Directory.
    
4. Passare al * * necessario eseguire altre attività * * pagina selezionare * * Troubleshoot * *, fare clic su **Avanti**. 
    
5. Nella pagina di risoluzione dei problemi, fare clic sul menu **Avvia per avviare la risoluzione dei problemi** di PowerShell. 
    
6. Nel menu principale, selezionare **La sincronizzazione delle Password risolvere i problemi**. 
    
7. Nel menu sub, selezionare **la sincronizzazione delle Password non funziona affatto**. 
    
 **Acquisire familiarità con i risultati dell'attività di risoluzione dei problemi**
  
L'attività di risoluzione dei problemi consente di eseguire le verifiche seguenti:
  
- Consente di verificare che la funzionalità di sincronizzazione password è abilitata per il tenant di Azure Active Directory.
    
- Convalida che il server di connessione di Azure Active Directory non è in modalità di gestione temporanea.
    
- Per ogni locale Active Directory connettore esistente (che corrisponde a una foresta di Active Directory esistente):
    
- 
  - Consente di verificare che sia abilitata la funzionalità di sincronizzazione delle password.
    
  - Cerca password sincronizzazione heartbeat eventi nei registri eventi applicazioni di Windows.
    
  - Per ogni dominio di Active Directory con il connettore di Active Directory locale:
    
  - Verifica che il dominio sia raggiungibile dal server di Azure Active Directory Connetti.
    
  - Consente di verificare che gli account di servizi di dominio Active Directory (AD DS) utilizzati dal connettore di Active Directory locale con la corretta username, password e le autorizzazioni necessarie per la sincronizzazione delle password.
    
Per ulteriore assistenza nella risoluzione dei problemi di sincronizzazione delle password, vedere [Troubleshoot la sincronizzazione delle password con sincronizzazione di Azure Active Directory Connetti](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).
  

