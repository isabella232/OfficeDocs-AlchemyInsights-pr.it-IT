---
title: Creare un sito in SharePoint Online
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
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: eaf09aebad5568aab3a716ce28c8ce3357c9f43175e1b1458bfcd43fd95a71fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057970"
---
# <a name="create-sharepoint-sites-using-templates"></a>Creare SharePoint siti con modelli

La possibilità di salvare un sito come modello non è supportata con le comunicazioni moderne o i siti del team. Per altre informazioni sull'utilizzo dei modelli, vedere [Salvare, scaricare e caricare un sito SharePoint come modello](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).

Ecco alcuni problemi/soluzioni comuni relativi al salvataggio di un sito o di un elenco come modello in Sharepoint Online. 

**Pulsante Salva sito/modello di elenco non disponibile o mancante**

Gli amministratori dovranno consentire agli script personalizzati di abilitare le funzionalità del modello. Per la procedura dettagliata, esempi e considerazioni, vedere 

- [Consentire o impedire lo script personalizzato](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Il comando Salva sito come modello non è supportato e può generare problemi nei siti che usano l'infrastruttura di pubblicazione di SharePoint Server.

**Il modello di sito non può essere creato o non funziona correttamente**

È possibile che nel modello non sia [presente una funzionalità](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) e che non venga attivata. Se la caratteristica non è disponibile per l'attivazione nella raccolta siti corrente, non è possibile usare il modello di sito per creare un sito.

- Verificare se eventuali elenchi o raccolte superano la [Soglia del limite di visualizzazione dell'elenco](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) di 5000 voci, poiché questo potrebbe bloccare la creazione di un modello di sito.

- Il sito potrebbe usare troppe risorse e pertanto il modello di sito supera il limite di 50 MB.


- La visualizzazione dei dati di un elenco che usa una colonna di ricerca presenta dei problemi. Per altre informazioni, vedere [Un elenco generato da un modello non visualizza i dati dell'elenco di ricerca corretto in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

Per informazioni più dettagliate su problemi e soluzioni comuni, vedere [Creare e utilizzare modelli di sito.](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)



