---
title: Di sola lettura per il messaggio di manutenzione quando si tenta di utilizzare SharePoint o OneDrive
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: cc232fba6f502e2b6f282a8c1a1e29221e36b70d
ms.sourcegitcommit: a285c609319ade038461e090e14a701830031825
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840519"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Di sola lettura per il messaggio di manutenzione quando si tenta di utilizzare SharePoint o OneDrive

Gli utenti possono ricevere un messaggio **di sola lettura per la manutenzione** quando si tenta di utilizzare SharePoint o OneDrive.  In caso affermativo, controllare se è presente una manutenzione attiva sul tenant passando al [centro messaggi](https://portal.office.com/adminportal/home#/MessageCenter). Assicurarsi inoltre di controllare il dashboard dell' [integrità del servizio](https://portal.office.com/adminportal/home#/servicehealth) per verificare la disponibilità di eventuali avvisi/incidenti che potrebbero verificarsi.

Se né il centro messaggi o il dashboard di integrità del servizio hanno rilevato nulla sulla manutenzione corrente per il tenant, potrebbe trattarsi di un problema relativo alla memorizzazione nella cache del browser.

Provare a cancellare la cache del browser prima di passare al sito.

1. Nel browser Microsoft Edge, selezionare **Impostazioni**, quindi selezionare **privacy e sicurezza**.
2. In **Pulisci esplorazione**, seleziona **Scegli cosa cancellare**.
3. Selezionare **cookie e dati del sito Web salvati**e selezionare **Annulla**.

>[!Note] 
> Questa procedura può essere diversa quando si utilizzano altri browser come Mozilla Firefox o Google Chrome.

>[!Note] 
> Un'altra opzione consiste nell'aprire il sito di SharePoint o OneDrive in una nuova finestra di InPrivate.