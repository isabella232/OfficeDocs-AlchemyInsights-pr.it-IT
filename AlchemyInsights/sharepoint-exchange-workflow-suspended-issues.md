---
title: Introduzione a SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: 285c580d69efb369fa6a60066165123e3c91b0a7
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051645"
---
# <a name="workflows-in-sharepoint"></a>Flussi di lavoro in SharePoint

Se i flussi di lavoro di SharePoint non inviano messaggi di posta elettronica, è possibile che l'organizzazione abbia incontrato i limiti dei mittenti di Exchange Online.

Il messaggio di errore "flusso di lavoro è sospeso" può verificarsi se si dispone di uno degli elementi seguenti:

- Si dispone di un flusso di lavoro in SharePoint Online che utilizza il tipo di piattaforma per flussi di lavoro di SharePoint 2010 o SharePoint 2013.

- Il flusso di lavoro è configurato per inviare un messaggio di posta elettronica personalizzato a più di 200 utenti alla volta, più di 10.000 destinatari al giorno o più di 30 messaggi al minuto.

Quando si esegue il flusso di lavoro, il messaggio di posta elettronica non viene inviato e si nota il messaggio di errore, lo stato interno è impostato su sospeso o non è in grado di inviare a un destinatario viene visualizzato.

Per ulteriori informazioni, vedere l' [articolo](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running)seguente.

