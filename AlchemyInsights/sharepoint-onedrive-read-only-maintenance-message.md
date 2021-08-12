---
title: Read-Only per il messaggio manutenzione quando si tenta di utilizzare SharePoint o OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: edcdea2f5c0647b92c230dd1d86549173e72997fc885195cde688b3b17710a2c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53910550"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Read-Only per il messaggio manutenzione quando si tenta di utilizzare SharePoint o OneDrive

Gli utenti potrebbero ricevere **un messaggio** di sola lettura per manutenzione quando tentano di utilizzare SharePoint o OneDrive per uno degli scenari seguenti. 

-   Attività di manutenzione pianificata o attiva.  Controllarli accedendo al [Centro messaggi](https://portal.office.com/adminportal/home#/messagecenter).
-   Un evento imprevisto di servizio attivo ad alta priorità che potrebbe verificarsi. Controllare eventuali avvisi/eventi imprevisti accedendo a [Integrità servizio](https://portal.office.com/adminportal/home#/servicehealth).
-   Uno scenario di ripristino con correzione automatica secondario che potrebbe verificarsi a causa di eventi imprevisti nei server che potrebbero durare meno di 30 minuti o meno. 
    
    Non ci sono post del Centro messaggi o integrità del servizio per questi recuperti minori, ma dovresti tornare alla normalità molto presto.

In pochissime occasioni è stato rilevato che uno dei tre scenari sopra elencati è stato la causa e che il servizio è stato ripristinato, ma la cache del browser degli utenti non è stata cancellata.

Tentare di cancellare la cache del browser prima di passare al sito.

1. Nel browser Microsoft Edge, selezionare **Impostazioni** e quindi **selezionare Privacy e sicurezza.**
2. In **Cancella esplorazione** selezionare Scegli cosa **cancellare.**
3. Selezionare **Cookie e dati del sito Web salvati** e selezionare **Cancella.**

>[!Note] 
> Questi passaggi possono essere diversi quando si utilizzano altri browser, ad esempio Mozilla Firefox o Google Chrome.

>[!Note] 
> Un'altra opzione potrebbe essere aprire il SharePoint o OneDrive in una nuova finestra inPrivate.