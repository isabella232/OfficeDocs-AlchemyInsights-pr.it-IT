---
title: Limitare la modalità classica di SharePoint Online
ms.author: pebaum
author: Techwriter40
ms.date: 3/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 18d263593d99f24c3020336ae601df14dbbf5411
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 10/18/2019
ms.locfileid: "36752072"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a>Limitare la modalità classica di SharePoint Online

Alcune organizzazioni richiedono ancora l'esperienza in modalità classica. Anche se non vi sono piani per rimuovere la modalità classica a un livello granulare, non è più possibile limitare un'intera organizzazione (tenant) alla modalità classica per gli elenchi e le raccolte.

L'amministratore avrà le seguenti opzioni per gestire singoli elenchi e raccolte in modalità classica utilizzando switch di opt-out granulare che vengono forniti ai livelli seguenti:

- raccolta siti
- sito
- elenco
- libreria

Inoltre, gli elenchi che utilizzano determinate caratteristiche e personalizzazioni non supportate dalla versione moderna continueranno a essere automaticamente passati alla modalità classica.

A partire dal 1 ° aprile 2019, il processo di disabilitazione del livello tenant opt-out dell'elenco e delle raccolte moderne inizierà e continuerà fino al 31 maggio 2019.  Gli elenchi e le raccolte che si trovano in modalità classica a seguito dell'opt-out del tenant verranno automaticamente spostati in versione moderna.

Se si richiede la modalità classica, vedere [qui](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) altre informazioni e istruzioni di PowerShell PNP che descrivono le opzioni e gli [strumenti che è](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) possibile utilizzare oggi per utilizzare l'esperienza in modalità classica.
