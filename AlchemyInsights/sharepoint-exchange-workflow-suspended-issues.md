---
title: Introduzione a SharePoint Online
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: 4c0220dd2535a1ef41aeef99e2bfc3fe28bac03a
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/04/2019
ms.locfileid: "36751676"
---
# <a name="workflows-in-sharepoint"></a>Flussi di lavoro in SharePoint

Se i flussi di lavoro di SharePoint non inviano messaggi di posta elettronica, è possibile che l'organizzazione abbia incontrato i limiti dei mittenti di Exchange Online.

Il messaggio di errore "flusso di lavoro è sospeso" può verificarsi se si dispone di uno degli elementi seguenti:

- Si dispone di un flusso di lavoro in SharePoint Online che utilizza il tipo di piattaforma per flussi di lavoro di SharePoint 2010 o SharePoint 2013.

- Il flusso di lavoro è configurato per inviare un messaggio di posta elettronica personalizzato a più di 200 utenti alla volta, più di 10.000 destinatari al giorno o più di 30 messaggi al minuto.

Quando si esegue il flusso di lavoro, il messaggio di posta elettronica non viene inviato e si nota il messaggio di errore, lo stato interno è impostato su sospeso o non è in grado di inviare a un destinatario viene visualizzato.

Per ulteriori informazioni, vedere l' [articolo](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running)seguente.

