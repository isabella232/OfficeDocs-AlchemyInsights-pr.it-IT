---
title: Posizione dei dati
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: ec8fb91dfe77cb251579ce23eb0579b114b101d9
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627850"
---
# <a name="data-location"></a>Posizione dei dati

È possibile visualizzare il percorso del tenant di Office 365 nell'interfaccia di amministrazione o la connessione a Exchange Online tramite PowerShell.


**Interfaccia di amministrazione:**
1. Accedere all'interfaccia di [Amministrazione](https://admin.microsoft.com/Adminportal/Home).
2. Selezionare**il profilo dell'organizzazione** **delle impostazioni** > .
3. In **percorso dati**selezionare **Visualizza dettagli**.


**PowerShell**
1. Connettersi a Exchange Online tramite Windows PowerShell.
2. Eseguire il cmdlet [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) per visualizzare un elenco delle proprietà del tenant. 
3. Esaminare la proprietà IDOrganizzazione.

Quando si dispone del percorso dati per EXO e SPO, è possibile determinare il percorso dei dati per gli altri servizi da [cui si trovano i dati](https://products.office.com/where-is-your-data-located).