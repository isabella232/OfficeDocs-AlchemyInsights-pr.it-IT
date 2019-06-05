---
title: Creare e utilizzare una cassetta postale condivisa
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 1825cfd0a78a29734d0a5128e19acbfba9115d32
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/04/2019
ms.locfileid: "34717351"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Risoluzione dei problemi relativi a un utente non trovato nella directory

<p>Se gli utenti ricevono un messaggio <strong> &ldquo; &hellip;di errore&rsquo;, l'utente non può essere trovato nella directory. Provare di nuovo&hellip; </strong> in cui il tipo di problema è <strong> &ldquo;utente non presente&rdquo;nella directory.</strong>, è possibile completare i passaggi seguenti per risolvere il problema.</p> <ol> <li>Verificare che l'account che ha accettato l'invito alla posta elettronica sia lo stesso utilizzato per l'accesso in un secondo momento. Assicurarsi che l'utente stia utilizzando lo stesso account per accettare l'invito e accedere al sito. <br /><br />Per altre informazioni, vedere <a href="https://support.microsoft.com/en-us/help/12407/microsoft-account-how-to-manage-aliases">How to Manage aliases for your Microsoft account</a> to manage the Office 365 login. <br /><br /></li> <li>Passare a ogni sito o i siti in cui l'utente riceve l'errore. <br /><br />un. Aggiungere <strong> &ldquo;/_layouts/15/people.aspx/membershipgroupid = 0&rdquo; </strong> (tra virgolette doppie) alla fine dell'URL del sito. <br /><br />Esempio: https://&lt;contoso&gt;. SharePoint.com/_layouts/15/people.aspx/membershipGroupId=0 <br /><br />b. Selezionare l'utente dall'elenco. <br /><br />c. Fare clic su <strong>Rimuovi autorizzazioni utente dalla barra multifunzione</strong>. <br /><br />d. Aggiungere di nuovo l'utente e rinviare l'invito all'utente.</li> </ol>

