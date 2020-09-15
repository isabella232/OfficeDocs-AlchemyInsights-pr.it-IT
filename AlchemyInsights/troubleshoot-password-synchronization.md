---
title: Risoluzione dei problemi relativi alla sincronizzazione delle password
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
ms.openlocfilehash: 96f63f2ae8e5de246bce7fc15a9b2c3d604f2eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664930"
---
# <a name="troubleshoot-password-synchronization"></a>Risoluzione dei problemi relativi alla sincronizzazione delle password

Per risolvere i problemi di sincronizzazione delle password, iniziare a utilizzare questa attività per la risoluzione dei problemi di AAD Connect per determinare il motivo per cui le password non vengono sincronizzate. Per iniziare, passare a [Gestione sincronizzazione diretta](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. Aprire una nuova sessione di Windows PowerShell nel server Azure AD Connect e selezionare l'opzione **Esegui come amministratore** .

2. Eseguire Set-ExecutionPolicy RemoteSigned o Set-ExecutionPolicy Unrestricted.

3. Avviare la procedura guidata di Azure AD Connect.

4. Passare alla pagina attività aggiuntive > **risoluzione dei problemi**  >  **successiva**.

5. Selezionare **Avvia** per aprire il menu di risoluzione dei problemi di PowerShell.

6. Selezionare **risoluzione dei problemi relativi alla sincronizzazione delle password**.

    Il problema è in genere che non viene sincronizzata una password per un account utente specifico.

    **Note** La sincronizzazione delle password ha esito negativo se l'ultima sincronizzazione della password è stata completata qualche tempo fa.

Per ulteriori informazioni sulla risoluzione dei problemi relativi alla sincronizzazione delle password, vedere [Troubleshoot password hash Synchronization with Azure ad Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).