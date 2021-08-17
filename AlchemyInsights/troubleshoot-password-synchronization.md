---
title: Risolvere i problemi di sincronizzazione delle password
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
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: cb782c0d1dc396ee7a9f016afb9629a2cdee93d52f5408b7a73e576e783ebc0a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105757"
---
# <a name="troubleshoot-password-synchronization"></a>Risolvere i problemi di sincronizzazione delle password

Per risolvere i problemi di sincronizzazione delle password, iniziare a usare questa attività di Connessione AAD per determinare il motivo per cui le password non vengono sincronizzate. Per iniziare, vai a [Gestire la sincronizzazione diretta.](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement)  

1. Aprire una nuova Windows PowerShell sul server Connessione Azure AD e selezionare **l'opzione Esegui come** amministratore.

2. Eseguire Set-ExecutionPolicy RemoteSigned o Set-ExecutionPolicy Unrestricted.

3. Avviare la procedura guidata di Connessione Azure AD.

4. Passare alla pagina Attività aggiuntive > **Risoluzione dei problemi**  >  **successivi**.

5. Seleziona **Avvia** per aprire il menu di risoluzione dei problemi di PowerShell.

6. Selezionare **Risoluzione dei problemi di sincronizzazione delle password.**

    Il problema è in genere che una password non è sincronizzata per un account utente specifico.

    **Note** La sincronizzazione delle password ha esito negativo se l'ultima sincronizzazione delle password è stata eseguita da qualche tempo.

Per ulteriori informazioni sulla risoluzione dei problemi di sincronizzazione delle password, vedere [Risolvere i problemi di sincronizzazione dell'hash](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)delle password con Azure AD Connessione sincronizzazione.