---
title: Read-Only per il messaggio di manutenzione quando si tenta di utilizzare SharePoint o OneDrive
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
ms.openlocfilehash: 376b653b18857103586e25edd0ad6801a7bbe0a1
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329452"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Read-Only per il messaggio di manutenzione quando si tenta di utilizzare SharePoint o OneDrive

Gli utenti potrebbero ricevere **un messaggio** di sola lettura per manutenzione quando tentano di utilizzare SharePoint o OneDrive per uno degli scenari seguenti. 

-   Attività di manutenzione pianificata o attiva.  Controllarli accedendo al [Centro messaggi](https://portal.office.com/adminportal/home#/messagecenter).
-   Un evento imprevisto di servizio attivo ad alta priorità che potrebbe verificarsi. Controllare eventuali avvisi/eventi imprevisti accedendo a [Integrità servizio](https://portal.office.com/adminportal/home#/servicehealth).
-   Uno scenario di ripristino con correzione automatica secondario che potrebbe verificarsi a causa di eventi imprevisti nei server che potrebbero durare meno di 30 minuti o meno. 
    
    Non ci sono post di integrità del servizio o del Centro messaggi per questi recuperti secondari, ma dovresti tornare alla normalità molto presto.

In pochissime occasioni è stato rilevato che uno dei tre scenari sopra elencati è la causa e che il servizio è stato ripristinato, ma la cache del browser degli utenti non è stata cancellata.

Tentare di cancellare la cache del browser prima di passare al sito.

1. Nel browser Microsoft Edge, selezionare **Impostazioni** e quindi selezionare **Privacy e sicurezza.**
2. In **Cancella esplorazione** selezionare Scegli cosa **cancellare.**
3. Selezionare **Cookie e dati del sito Web salvati** e selezionare **Cancella.**

**Nota:** questi passaggi possono essere diversi quando si utilizzano altri browser, ad esempio Mozilla Firefox o Google Chrome.

**Nota:** un'altra opzione potrebbe essere aprire il SharePoint o OneDrive in una nuova finestra di InPrivate.