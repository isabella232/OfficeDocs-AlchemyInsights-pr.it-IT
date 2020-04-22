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
ms.openlocfilehash: c769c17796d805f88afb4d5b32adb7d4a9bb3ce0
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/21/2020
ms.locfileid: "43655286"
---
# <a name="data-location"></a>Posizione dei dati

È possibile visualizzare la posizione del tenant nell'interfaccia di amministrazione o connettersi a Exchange Online tramite PowerShell.


**Interfaccia di amministrazione:**
1. Accedere all'interfaccia di [Amministrazione](https://admin.microsoft.com/Adminportal/Home).
2. Selezionare**il profilo dell'organizzazione** **delle impostazioni** > .
3. In **percorso dati**selezionare **Visualizza dettagli**.


**PowerShell**
1. Connettersi a Exchange Online tramite Windows PowerShell.
2. Eseguire il cmdlet [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) per visualizzare un elenco delle proprietà del tenant. 
3. Esaminare la proprietà IDOrganizzazione.

Quando si dispone del percorso dati per EXO e SPO, è possibile determinare il percorso dei dati per gli altri servizi da [cui si trovano i dati](https://products.office.com/where-is-your-data-located).