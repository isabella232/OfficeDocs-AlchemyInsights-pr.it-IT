---
title: Introduzione a SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: a14705003f742641f10c8459b7c7024146e4134a8d5113451e5732cef7326484
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54051418"
---
# <a name="workflows-in-sharepoint"></a>Flussi di lavoro in SharePoint

Se SharePoint flussi di lavoro non inviano messaggi di posta elettronica, è possibile che l'organizzazione abbia riscontrato i limiti Exchange Online mittente.

Il messaggio di errore "Flusso di lavoro sospeso" può verificarsi se si dispone di uno degli elementi seguenti:

- Si dispone di un flusso di lavoro in SharePoint Online che usa il tipo SharePoint 2010 o SharePoint 2013.

- Il flusso di lavoro è configurato per inviare un messaggio di posta elettronica personalizzato a più di 200 utenti contemporaneamente, più di 10.000 destinatari al giorno o più di 30 messaggi al minuto.

Quando si esegue il flusso di lavoro, il messaggio di posta elettronica non viene inviato e si nota il messaggio di errore, Lo stato interno è impostato su Sospeso o Non è possibile inviare a un destinatario viene visualizzato.

Per ulteriori informazioni, fare riferimento all'articolo [seguente.](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running)

