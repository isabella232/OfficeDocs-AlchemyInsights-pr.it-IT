---
title: Impossibile eliminare elementi in SharePoint o OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: 3601c5eff121e10b6bddace6f7228204a01080a636e24f3a56373fe8d469c799
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038521"
---
# <a name="unable-to-delete-items"></a>Impossibile eliminare elementi

- I criteri di conservazione possono causare questo problema, è necessario disabilitare o escludere il rispettivo blocco che causa questo problema. Dopo la rimozione di un criterio di conservazione o di un blocco, l'applicazione della modifica potrebbe richiedere fino a 24 ore. Verificare che non sia presente [un'impostazione dei criteri](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) di conservazione per l'elemento.

- Il sito potrebbe aver superato il limite di archiviazione, aumentare la [quota del sito](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) ed eliminare l'elemento.

- Verificare che l'elemento non [sia estratto](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) da un altro utente.

- Infine, gli amministratori possono usare [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) che contiene una raccolta di comandi di PowerShell che consentono di eseguire azioni di gestione complesse, ad esempio forzare l'eliminazione di elementi testardi.
- [Rimuovi file PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Rimuovi cartella PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Rimuovi elemento elenco PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Rimuovi elenco PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Rimuovi campo PNP (colonna)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)