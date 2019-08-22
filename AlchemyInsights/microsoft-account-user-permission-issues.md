---
title: Risoluzione dei problemi relativi a un utente non trovato nella directory
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 537b27d06acd17cbb3fe99bcb89e153099e92bb4
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36544867"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Risoluzione dei problemi relativi a un utente non trovato nella directory

Se gli utenti ricevono il messaggio di errore "l'utente non può essere trovato" nella directory. Provare di nuovo in cui il tipo di problema è utente non presente nella directory.

Per risolvere il problema, è possibile completare i passaggi seguenti.

- Verificare che l'account che ha accettato l'invito alla posta elettronica sia lo stesso utilizzato per l'accesso in un secondo momento. Assicurarsi che l'utente stia utilizzando lo stesso account per accettare l'invito e accedere al sito. 

Per altre informazioni, vedere [How to Manage aliases for your Microsoft</a> account to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Passare a ogni sito o i siti in cui l'utente riceve l'errore. 

Aggiungere "/_layouts/15/people.aspx/membershipgroupid = 0" (tra virgolette doppie) alla fine dell'URL del sito. 

Esempio: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Selezionare l'utente dall'elenco.

- Fare clic su **Rimuovi autorizzazioni utente** dalla barra multifunzione. 
-  Aggiungere di nuovo l'utente e rinviare l'invito all'utente.

