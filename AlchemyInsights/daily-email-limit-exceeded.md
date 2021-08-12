---
title: Limite giornaliero di posta elettronica superato. Flusso di lavoro sospeso.
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
- "5200020"
- "1227"
ms.openlocfilehash: 60ddbe68298e998a4e0b271a15209efc135c80638702c98dbcb3e0b2f1554860
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53914655"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Limite giornaliero di posta elettronica superato. Flusso di lavoro sospeso.

Questo errore può essere ricevuto negli scenari seguenti:

- Si dispone di un flusso di lavoro in SharePoint Online che usa il tipo SharePoint 2010 o SharePoint 2013.
- Il flusso di lavoro è configurato per inviare un messaggio di posta elettronica personalizzato a più di 200 utenti contemporaneamente, più di 10.000 destinatari al giorno o più di 30 messaggi al minuto.
- Quando si esegue il flusso di lavoro, il messaggio di posta elettronica non viene inviato e si nota il comportamento seguente:
    - Per un flusso di lavoro SharePoint 2013, passare alla pagina **Stato flusso di** lavoro. Nella pagina Stato flusso di lavoro lo **stato** interno è impostato su **Avviato** e nell'area informazioni viene visualizzato **Impossibile inviare a un destinatario**.

Per risolvere questo problema, configurare il flusso di lavoro per l'invio di messaggi di posta elettronica senza superare i Exchange Online [mittente.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits) Ad esempio, utilizzare una pausa nel flusso di lavoro, inviare il messaggio di posta elettronica a un gruppo di Microsoft 365, a un gruppo di distribuzione o a un gruppo di sicurezza abilitato alla posta oppure inviare il messaggio a meno di 200 destinatari alla volta.


Per ulteriori informazioni, vedere l'articolo [seguente.](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)

## <a name="related-topics"></a>Argomenti correlati
- [Creare Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint e Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 