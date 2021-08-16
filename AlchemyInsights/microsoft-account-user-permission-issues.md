---
title: Risolvere il problema - Utente non trovato nella directory
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 79429f8e9523ad6b08cd2cd2b19dd221bac797d00de142cbb18826b86fb5ae4e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098174"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Risolvere il problema - Utente non trovato nella directory

Se gli utenti ricevono il messaggio di errore "Impossibile trovare l'utente" nella directory, riprovare dove Tipo problema è Utente non in directory.

I passaggi seguenti possono essere completati per risolvere il problema.

- Verificare che l'account che ha accettato l'invito tramite posta elettronica sia lo stesso account utilizzato per accedere in un secondo momento. Assicurati che l'utente utilizzi lo stesso account per accettare l'invito e accedere al sito. 

Per altre info, vedi Come gestire gli alias per il tuo account Microsoft per [ </a> gestire l'Microsoft 365 accesso.](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases) 

- Passare a ogni sito in cui l'utente riceve l'errore. 

Aggiungere "/_layouts/15/people.aspx/membershipgroupid=0" (tra virgolette doppie) alla fine dell'URL del sito. 

Esempio: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Selezionare l'utente dall'elenco.

- Fare **clic su Rimuovi autorizzazioni utente** dalla barra multifunzione. 
-  Aggiungere di nuovo l'utente e inviare di nuovo l'invito all'utente.

