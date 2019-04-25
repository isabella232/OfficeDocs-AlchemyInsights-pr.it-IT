---
title: La condivisione con utenti esterni non funziona
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 69e290e5a13f40ad045086791189a7d0af88240b
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32369502"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Risolvere i problemi di condivisione del contenuto di SharePoint con utenti esterni

Verificare che la condivisione esterna sia attivata per l'organizzazione:
  
1. Passare alla [pagina componenti &amp; aggiuntivi servizi nell'interfaccia di amministrazione di Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)e quindi fare clic su **siti**.
    
2. Verificare che l'impostazione sia attivata su "attivo". Se è selezionata l'opzione "solo utenti esterni esistenti", verificare che l'utente esterno sia elencato nell'interfaccia di amministrazione di Microsoft 365.
    
Assicurarsi che la condivisione esterna sia attivata per il sito. Per una raccolta siti classica:
  
1. Nel riquadro sinistro della nuova interfaccia di amministrazione di SharePoint fare clic su **siti**.
    
2. Selezionare il sito o i siti e sulla barra multifunzione fare clic su **condivisione**.
    
Per un sito del team che appartiene a un gruppo di Office 365 o a un sito di comunicazione:
  
- Questi nuovi tipi di sito hanno la stessa impostazione di condivisione dell'impostazione a livello di organizzazione, a meno che l'impostazione a livello di organizzazione non consenta la condivisione dei file tramite collegamenti che non richiedono l'accesso. In questo caso, i siti consentono la condivisione con utenti esterni nuovi ed esistenti che effettuano l'accesso. Per modificare l'impostazione per siti specifici, utilizzare la nuova interfaccia di amministrazione di SharePoint o PowerShell. [Altre informazioni](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> L'impostazione di condivisione esterna per qualsiasi sito può essere più restrittiva rispetto all'impostazione a livello dell'organizzazione, ma non più permissiva rispetto all'impostazione a livello dell'organizzazione. 
  

