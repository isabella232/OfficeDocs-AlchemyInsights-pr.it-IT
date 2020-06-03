---
title: Impossibile eliminare gli elementi in SharePoint o OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: 8647b65c52a782ca48ca58bb2700556db528796b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511980"
---
# <a name="unable-to-delete-items"></a>Impossibile eliminare gli elementi

I criteri di conservazione possono causare questa operazione, è necessario disabilitare o escludere il blocco corrispondente che causa questo problema. Dopo la rimozione di un criterio di conservazione o di un blocco, potrebbero essere necessarie fino a 24 ore per rendere effettive le modifiche. Verificare che non vi sia una configurazione dei [criteri di conservazione](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) per l'elemento.

Il sito potrebbe avere superato il limite di archiviazione, aumentare la [quota del sito](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) ed eliminare l'elemento.

Verificare che l'elemento non venga [Estratto](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) da un altro utente.

Infine, gli amministratori possono utilizzare [le procedure e i modelli di SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PNP) che contengono una raccolta di comandi di PowerShell che consentono di eseguire azioni di gestione complesse, ad esempio forza eliminando gli elementi ostinati.
- [Rimuovi file PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Rimuovi cartella PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Rimuovi elemento dell'elenco PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Rimuovi elenco PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Rimuovi campo PNP (colonna)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)