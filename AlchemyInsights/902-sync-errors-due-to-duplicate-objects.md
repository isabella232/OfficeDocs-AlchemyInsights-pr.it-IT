---
title: 902 (gli errori di sincronizzazione a causa di oggetti duplicati)
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: f576460547110e0e599a9062ae03f690792fe635
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29919876"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Errori di sincronizzazione a causa di oggetti duplicati

Al termine della sincronizzazione della directory, è possibile ricevere uno dei seguenti messaggi di errore:
  
- Non è possibile aggiornare l'oggetto in Microsoft Online Services, in quanto gli attributi seguenti associati all'oggetto hanno i valori che possono essere già associati a un altro oggetto nella directory locale.
    
- Un oggetto sincronizzato con lo stesso indirizzo proxy esiste già nella directory di Microsoft Online Services.
    
- Non è possibile aggiornare l'oggetto perché i seguenti attributi associati all'oggetto dispongono di valori che possono essere già associati a un altro oggetto in servizi directory locale: UserPrincipalName.
    
Per identificare e correggere il problema, scaricare ed eseguire lo [Strumento di risoluzione dei problemi di IdFix DirSync errore](https://www.microsoft.com/download/details.aspx?id=36832).
  
Per ulteriori informazioni, vedere [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
  

