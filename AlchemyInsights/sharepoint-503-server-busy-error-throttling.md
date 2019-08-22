---
title: Limitazione di SharePoint Online
ms.author: kirks
author: Techwriter40
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: c7881c0c7331e0aa74fcc439f52157bb75a56160
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36559845"
---
# <a name="sharepoint-online-throttling"></a>Limitazione di SharePoint Online

Gli utenti possono ricevere un server 503 è un errore durante il tentativo di accedere a siti di SharePoint o OneDrive. 

Questo errore può essere causato dalla limitazione all'interno del servizio di SharePoint. SharePoint Online utilizza la limitazione per mantenere le prestazioni ottimali e l'affidabilità del servizio SharePoint Online. La limitazione limita il numero di azioni utente o di chiamate simultanee (tramite script o codice) per impedire un utilizzo eccessivo delle risorse. Se si ottiene la limitazione, il 99% del tempo è a causa del codice personalizzato.

Per ulteriori informazioni sulla limitazione, vedere [impedire la limitazione o il blocco in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

Se si ritiene che questo errore non sia correlato alla limitazione, è possibile controllare se è presente una manutenzione attiva sul tenant passando al [centro messaggi](https://portal.office.com/adminportal/home#/MessageCenter).

 Infine, verificare di aver visitato la pagina di [integrità del servizio](https://portal.office.com/adminportal/home#/servicehealth) per controllare eventuali avvisi/incidenti che potrebbero verificarsi.

