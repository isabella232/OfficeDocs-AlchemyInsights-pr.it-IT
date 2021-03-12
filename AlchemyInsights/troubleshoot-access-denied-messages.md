---
title: Risoluzione dei problemi relativi ai messaggi di accesso negato
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 6c8ad84123fb58b73b9c378592ce970997893ea2
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704898"
---
# <a name="troubleshoot-access-denied-messages"></a>Risoluzione dei problemi relativi ai messaggi di accesso negato

Se un utente ha ricevuto un messaggio "Accesso negato" a una cartella condivisa in SharePoint, l'amministratore della raccolta siti potrebbe aver abilitato la "modalità di blocco delle autorizzazioni utente con accesso limitato". Per disattivare questa opzione: 
  
1. Passare al sito, fare clic sull'icona Impostazioni e quindi su **Impostazioni sito.**
    
2. In **Amministrazione raccolta siti** fare clic su **Caratteristiche raccolta siti**.
    
3. Accanto a **Modalità di blocco delle autorizzazioni utente** con accesso limitato fare clic su **Disattiva.**
    
È inoltre possibile che per le cartelle condivise si verifichi un messaggio di accesso negato se il sito è un sito di pubblicazione. Per informazioni, vedere [Accesso negato quando si accede a una cartella condivisa.](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb)
  
Se un utente ha ricevuto un messaggio "Accesso negato" quando tenta di visualizzare le richieste di accesso, l'utente deve essere aggiunto come amministratore della raccolta siti o come membro del gruppo Proprietari del sito. Per altre info, vedi [l'elenco Access Denied to Access Requests.](https://go.microsoft.com/fwlink/?linkid=2004220)
  
Se un utente ha ricevuto un messaggio "Accesso negato" dopo essere stato rimosso da Active Directory locale e quindi aggiunto nuovamente, vedere Accesso negato quando un account utente viene sincronizzato con [Microsoft 365.](https://go.microsoft.com/fwlink/?linkid=2004318)
  

