---
title: Superamento del limite di posta elettronica giornaliero. Il flusso di lavoro è sospeso.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 3cad5d8305da0a5db9a85888793350a062e6aed6
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053121"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Superamento del limite di posta elettronica giornaliero. Il flusso di lavoro è sospeso.

Questo errore può essere ricevuto negli scenari seguenti:

- Si dispone di un flusso di lavoro in SharePoint Online che utilizza il tipo di piattaforma per flussi di lavoro di SharePoint 2010 o SharePoint 2013.
- Il flusso di lavoro è configurato per inviare un messaggio di posta elettronica personalizzato a più di 200 utenti alla volta, più di 10.000 destinatari al giorno o più di 30 messaggi al minuto.
- Quando si esegue il flusso di lavoro, il messaggio di posta elettronica non viene inviato e si nota il comportamento seguente:
    - Per un flusso di lavoro che utilizza il tipo di piattaforma SharePoint 2013, passare alla pagina **stato flusso di lavoro** . Nella pagina Stato flusso di lavoro lo **stato interno** è impostato su **avviato**e il fumetto di informazioni non è in **grado di inviare messaggi a un destinatario**.

Per ovviare a questo problema, configurare il flusso di lavoro per l'invio di messaggi di posta elettronica senza superare i [limiti dei mittenti di Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Ad esempio, utilizzare una pausa nel flusso di lavoro, inviare il messaggio di posta elettronica a un gruppo di Office 365, a un gruppo di distribuzione o di sicurezza abilitato alla posta elettronica oppure inviare i messaggi a un numero di destinatari inferiore a 200 alla volta.


Per ulteriori informazioni, vedere l' [articolo](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)seguente.

## <a name="related-topics"></a>Argomenti correlati
- [Crea flusso](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint e flusso](https://flow.microsoft.com/blog/sharepoint-and-flow/) 