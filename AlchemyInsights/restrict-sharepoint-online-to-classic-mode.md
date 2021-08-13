---
title: Limitare SharePoint Online alla modalità classica
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 6315a83ac825f96ceea60798d441de8e8e53336fe29eda4d0491dd8a6a43b352
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53958805"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a>Limitare SharePoint Online alla modalità classica

Alcune organizzazioni richiedono comunque l'esperienza in modalità classica. Anche se non sono disponibili piani per rimuovere la modalità classica a livello granulare, non è più possibile limitare un'intera organizzazione (tenant) alla modalità classica per elenchi e raccolte.

L'amministratore avrà le opzioni seguenti per gestire singoli elenchi e raccolte in modalità classica usando opzioni di rifiuto esplicito granulari fornite ai livelli seguenti:

- raccolta siti
- site
- list
- library

Inoltre, gli elenchi che utilizzano determinate caratteristiche e personalizzazioni non supportate dalla versione moderna verranno comunque automaticamente visualizzati in modalità classica.

A partire dal 1° aprile 2019, il processo di disattivazione del livello tenant per rifiutare esplicitamente l'elenco e le raccolte moderne inizierà e continuerà fino al 31 maggio 2019.  Gli elenchi e le raccolte che sono in modalità classica a seguito del rifiuto esplicito del tenant verranno automaticamente spostati alla modalità moderna.

Se è necessaria la modalità [](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) classica, vedere altre [](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) informazioni qui e istruzioni su PowerShell PnP che descrivono le opzioni e gli strumenti che è possibile usare oggi per usare l'esperienza in modalità classica.
