---
title: La condivisione con utenti esterni non funziona
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: bd3a6c0d7206801ff76be121c4878b8343cc9886
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691579"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Risolvere i problemi di condivisione del contenuto di SharePoint con utenti esterni

Verificare che la condivisione esterna sia attivata per l'organizzazione:
  
1. Passare alla [ &amp; pagina componenti aggiuntivi servizi nell'interfaccia di amministrazione di Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)e quindi fare clic su **siti**.
    
2. Verificare che l'impostazione sia attivata su "attivo". Se è selezionata l'opzione "solo utenti esterni esistenti", verificare che l'utente esterno sia elencato nell'interfaccia di amministrazione di Microsoft 365.
    
Assicurarsi che la condivisione esterna sia attivata per il sito. Per una raccolta siti classica:
  
1. Nel riquadro sinistro della nuova interfaccia di amministrazione di SharePoint fare clic su **siti**.
    
2. Selezionare il sito o i siti e sulla barra multifunzione fare clic su **condivisione**.
    
Per un sito del team che appartiene a un gruppo di Microsoft 365 o a un sito di comunicazione:
  
- Questi nuovi tipi di sito hanno la stessa impostazione di condivisione dell'impostazione a livello di organizzazione, a meno che l'impostazione a livello di organizzazione non consenta la condivisione dei file tramite collegamenti che non richiedono l'accesso. In questo caso, i siti consentono la condivisione con utenti esterni nuovi ed esistenti che effettuano l'accesso. Per modificare l'impostazione per siti specifici, utilizzare la nuova interfaccia di amministrazione di SharePoint o PowerShell. [Altre informazioni](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> L'impostazione di condivisione esterna per qualsiasi sito può essere più restrittiva rispetto all'impostazione a livello dell'organizzazione, ma non più permissiva rispetto all'impostazione a livello dell'organizzazione. 
  

