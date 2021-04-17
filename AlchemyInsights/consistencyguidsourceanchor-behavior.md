---
title: Comportamento di ConsistencyGuid/sourceAnchor
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: eafe1ec9636cddc9d73a88beb7ae3ad9f6fad660
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816996"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>Comportamento di ConsistencyGuid/sourceAnchor

Azure AD Connect (versione 1.1.524.0 e successiva) ora facilita l'uso di msDS-ConsistencyGuid come attributo sourceAnchor. Quando si usa questa funzionalità, Azure AD Connect configura automaticamente le regole di sincronizzazione per:
  
- Utilizzare msDS-ConsistencyGuid come attributo sourceAnchor per gli oggetti User. ObjectGUID viene utilizzato per altri tipi di oggetto.
    
- Per qualsiasi oggetto utente AD locale il cui attributo msDS-ConsistencyGuid non è popolato, Azure AD Connect scrive il valore objectGUID nell'attributo msDS-ConsistencyGuid in Active Directory locale. Dopo aver popolato l'attributo msDS-ConsistencyGuid, Azure AD Connect esporta quindi l'oggetto in Azure AD.
    
 **Nota:** Dopo l'importazione di un oggetto AD locale in Azure AD Connect, ovvero importato nello spazio connettore AD e proiettato nel Metaverse, non è più possibile modificarne il valore sourceAnchor. Per specificare il valore sourceAnchor per un determinato oggetto AD locale, configurare il relativo attributo msDS-ConsistencyGuid prima di importarlo in Azure AD Connect. 
  
Per altre informazioni su SourceAnchor e ConsistencyGuid, fare riferimento a: [Azure AD Connect: Concetti di progettazione](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

