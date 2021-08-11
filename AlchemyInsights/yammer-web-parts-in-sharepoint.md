---
title: Web part di Yammer in SharePoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5475"
- "9002494"
ms.openlocfilehash: a252dab703e639c7c11fe6aead1db04aeecfe54bc6d52bcd4a28433aed4701d5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53970335"
---
# <a name="yammer-web-parts-in-sharepoint"></a>Web part di Yammer in SharePoint

Le web part delle Conversazioni di Yammer e degli Elementi salienti di Yammer rafforza la collaborazione sulle pagine di SharePoint moderne e classiche. Per altre informazioni, vedere [Conversazioni di Yammer](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#conversations) ed [Elementi salienti di Yammer](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#highlights).    

La web part delle Conversazioni di Yammer è in fase di aggiornamento alla nuova esperienza di Yammer ed è disponibile per i tenant di rilascio mirato. L'implementazione di GA è iniziata. Le nuove funzionalità includono la possibilità di avviare una conversazione con qualsiasi post, (Domande, Sondaggi, Complimento) e inviare le risposte migliori direttamente da SharePoint. Per ulteriori informazioni, vedere [Domande frequenti e Condizioni per i clienti sul nuovo Yammer](https://docs.microsoft.com/yammer/get-started-with-yammer/newyammer-faq).

 Per informazioni sulle web part e sulla configurazione appropriate, vedere [Usare una Web part Yammer in SharePoint Online](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da).  

**Uso delle web part con SharePoint Server**  

È possibile usare le web part nelle pagine moderne e classiche negli ambienti locali.

- Per altre informazioni sulle pagine moderne, vedere [Aggiungere un feed di Yammer a una pagina moderna in SharePoint Server 2019](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-modern-page-in-sharepoint-server-2019). 
- Per altre informazioni sulle pagine classiche, vedere [Aggiungere un feed di Yammer a una pagina moderna in SharePoint Server 2013, 2016 e 2019](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-classic-page-in-sharepoint-servers-2013-2016-and-2019).

**Yammer Embed**  

Usare lo strumento di configurazione Incorpora per testarne l'utilizzo. Un aggiornamento futuro di Incorpora abiliterà la nuova esperienza di Yammer. Per altre informazioni, vedere lo [Strumento di configurazione di Yammer Embed](https://aka.ms/YammerEmbedConfigureTool). Per comprendere meglio il componente Incorpora, vedere [il feed Incorpora](https://aka.ms/YammerDevDocs).

**Problemi noti e risoluzioni**

- Gli ID gruppo non sono disponibili dai nuovi URL di Yammer, che sono stati modificati. Tornare alla modalità classica per ottenere gli ID del gruppo o altri ID degli URL.
- I domini personalizzati non sono supportati.
- Yammer Embed non è ottimizzato per dispositivi mobili. Usare le pagine moderne con la web part delle Conversazioni di Yammer per un'esperienza ottimale.
- I temi personalizzati possono influire sull'aspetto e sulla fruibilità della web part delle Conversazioni di Yammer. Aprire un caso di supporto per segnalare i problemi.