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
ms.openlocfilehash: b554bfa4ccccbd68d0c3df27cf17397f860735c2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732231"
---
# <a name="create-sharepoint-sites-using-templates"></a>Creare siti di SharePoint mediante modelli

La possibilità di salvare un sito come modello non è supportata con i siti di comunicazione o di Team moderni. Per ulteriori informazioni sull'utilizzo dei modelli [, vedere Salvataggio, download e caricamento di un sito di SharePoint come modello](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).

Di seguito sono riportate alcune soluzioni o problemi comuni relativi al salvataggio di un sito o di un elenco come modello in SharePoint Online. 

**Il pulsante Salva modello di sito/elenco non è disponibile o mancante**

Gli amministratori dovranno consentire lo script personalizzato per abilitare le caratteristiche del modello. Per la procedura dettagliata, esempi e considerazioni vedere 

- [Consentire o impedire lo script personalizzato](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Il comando Salva sito come modello non è supportato e può causare problemi nei siti che utilizzano l'infrastruttura di pubblicazione di SharePoint Server.

**Il modello di sito non può essere creato o non funziona correttamente**

Il modello può mancare una [funzionalità](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) e non viene attivato. Se la funzionalità non è disponibile per l'attivazione nella raccolta siti corrente, non è possibile utilizzare il modello di sito per creare un sito.

- Controllare se gli elenchi o le raccolte superano la [soglia di limite per la visualizzazione elenco](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) di 5000 elementi, in quanto è possibile bloccare la creazione di un modello di sito.

- Il sito può utilizzare troppe risorse e quindi il modello di sito supera il limite di 50 MB.


- Sono presenti problemi durante la visualizzazione di dati da un elenco che utilizza una colonna di ricerca. Per ulteriori informazioni, vedere [elenco generato da modelli non Visualizza i dati dell'elenco di ricerca corretto in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

Per informazioni più dettagliate su problemi e soluzioni comuni, vedere [creare e utilizzare modelli di sito](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



