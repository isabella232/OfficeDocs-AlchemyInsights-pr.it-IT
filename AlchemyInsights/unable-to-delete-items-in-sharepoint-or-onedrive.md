---
title: Impossibile eliminare gli elementi in SharePoint o OneDrive
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 21d7b928fade48a6729c120e6ea33b16dafe799e
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057732"
---
# <a name="unable-to-delete-items"></a>Impossibile eliminare gli elementi

Problemi relativi all'eliminazione di elementi?

- Assicurarsi sempre di disporre delle [autorizzazioni appropriate](https://docs.microsoft.com/en-us/sharepoint/default-sharepoint-groups) per eliminare l'elemento oppure che il tentativo di amministratore di una [raccolta siti](https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) sia stato rimosso.

- Verificare che non vi sia una configurazione dei [criteri di conservazione](https://docs.microsoft.com/en-us/office365/securitycompliance/retention-policies) per l'elemento.

- Verificare che l'elemento non venga [Estratto](https://support.office.com/en-us/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) da un altro utente.

- Infine, gli amministratori possono utilizzare [le procedure e i modelli di SharePoint](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PNP) che contengono una raccolta di comandi di PowerShell che consentono di eseguire azioni di gestione complesse, ad esempio forza eliminando gli elementi ostinati. 
- [Rimuovi file PNP](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Rimuovi cartella PNP](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Rimuovi elemento dell'elenco PNP](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Rimuovi elenco PNP](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Rimuovi campo PNP (colonna)](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)