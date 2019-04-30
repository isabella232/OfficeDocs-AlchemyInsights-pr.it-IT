---
title: Salvare il sito o l'elenco come modello
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 7930551c0938501d006f791491594f9d6d9ba260
ms.sourcegitcommit: 03258ec4f5476a1ea6dd3a31d17bda815bc5a18a
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/24/2019
ms.locfileid: "33243459"
---
# <a name="save-site-or-list-as-a-template"></a>Salvare il sito o l'elenco come modello

I modelli di sito di SharePoint sono definizioni predefinite progettate attorno a una specifica esigenza aziendale. Per ulteriori informazioni, vedere [utilizzo di modelli per creare diversi tipi di siti di SharePoint](https://support.office.com/en-us/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Di seguito sono riportate alcune soluzioni o problemi comuni relativi al salvataggio di un sito o di un elenco come modello in SharePoint Online.

Il **pulsante Salva modello di sito/elenco non è disponibile o mancante**. 

- Gli amministratori dovranno consentire lo script personalizzato per abilitare le caratteristiche del modello. Per la procedura dettagliata, esempi e considerazioni, vedere [Allow or impedisce script personalizzato](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).


- Il comando Salva sito come modello non è supportato e può causare problemi nei siti che utilizzano l'infrastruttura di pubblicazione di SharePoint Server.


**Il modello di sito non può essere creato o non funziona correttamente**

- Il modello può mancare una [funzionalità](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) e non viene attivato. Se la funzionalità non è disponibile per l'attivazione nella raccolta siti corrente, non è possibile utilizzare il modello di sito per creare un sito.


- Controllare se gli elenchi o le raccolte superano la [soglia di limite per la visualizzazione elenco](https://support.office.com/en-us/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) di 5000 elementi, in quanto è possibile bloccare la creazione di un modello di sito.


- Il sito può utilizzare troppe risorse e quindi il modello di sito supera il limite di 50 megabyte (MB).


- Sono presenti problemi durante la visualizzazione di dati da un elenco che utilizza una colonna di ricerca. Per ulteriori informazioni, vedere [elenco generato da modelli non Visualizza i dati dell'elenco di ricerca corretto in SharePoint Online](https://support.office.com/en-us/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).


Per informazioni più dettagliate su problemi e soluzioni comuni, fare riferimento, [creare e utilizzare modelli di sito](https://support.office.com/en-us/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).
