---
title: Sito moderno come sito radice
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 6166493f79379f44b1a9bbbaca6becfe624fe912
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057731"
---
# <a name="modern-site-as-root-site"></a>Sito moderno come sito radice

I clienti di [release di destinazione](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) possono ora abilitare la moderna esperienza del sito di comunicazione nel sito radice classico del tenant di SharePoint.

Questa funzionalità può essere attivata eseguendo un semplice cmdlet di PowerShell. Per l'esecuzione corretta dei comandi di PowerShell, il sito radice avrà una nuova Home page del sito di comunicazione. Informazioni dettagliate sul cmdlet e sui requisiti di funzionalità di PowerShell sono disponibili nell'articolo [Enable-SPOCommSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps). 

In questo modo, per impostazione predefinita, verranno implementati i clienti di release mirati all'inizio di maggio 2019 e il lancio sarà disponibile in tutto il mondo entro la fine del 2019 giugno. Continuare a fare riferimento al [centro messaggi](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) per altre nuove funzionalità con Modern. 

**Importante**: non eliminare il sito radice classico per creare un sito di comunicazione moderno. Questo non è supportato da Microsoft. L'eliminazione del sito radice renderà tutti i siti di SharePoint dell'organizzazione inaccessibili a tutti gli utenti, fino a quando non si ripristina il sito o si crea un nuovo sito nello stesso URL. 
 
 