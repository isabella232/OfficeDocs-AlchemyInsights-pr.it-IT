---
title: Salvare un sito o un elenco come modello
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 31cb294be6b72be313cf63ed5ed2af0ef041dcf6efb7a7a2af4e1b6a9a149c43
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54109208"
---
# <a name="save-site-or-list-as-a-template"></a>Salvare un sito o un elenco come modello

SharePoint modelli di sito sono definizioni predefinite progettate in base a specifiche esigenze aziendali. Per ulteriori informazioni, vedere [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Ecco alcuni problemi/soluzioni comuni relativi al salvataggio di un sito o di un elenco come modello in SharePoint Online.

**Il pulsante Salva modello di sito/elenco non è disponibile o mancante.** 

- Gli amministratori dovranno consentire agli script personalizzati di abilitare le funzionalità del modello. Per la procedura dettagliata, gli esempi e le considerazioni, [vedere Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


- Il comando Salva sito come modello non è supportato e può generare problemi nei siti che usano l'infrastruttura di pubblicazione di SharePoint Server.


**Il modello di sito non può essere creato o non funziona correttamente**

- È possibile che nel modello non sia [presente una funzionalità](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) e che non venga attivata. Se la caratteristica non è disponibile per l'attivazione nella raccolta siti corrente, non è possibile usare il modello di sito per creare un sito.


- Verificare se eventuali elenchi o raccolte superano la [Soglia del limite di visualizzazione dell'elenco](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) di 5000 voci, poiché questo potrebbe bloccare la creazione di un modello di sito.


- Il sito potrebbe utilizzare troppe risorse e pertanto il modello di sito supera il limite di 50 MEGABYTE (MB).


- La visualizzazione dei dati di un elenco che usa una colonna di ricerca presenta dei problemi. Per ulteriori informazioni, vedere [Template-generated list doesn't display data from the correct lookup list in SharePoint Online.](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data)


Per informazioni più dettagliate su problemi e soluzioni comuni, vedere [Creare e utilizzare modelli di sito.](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)

