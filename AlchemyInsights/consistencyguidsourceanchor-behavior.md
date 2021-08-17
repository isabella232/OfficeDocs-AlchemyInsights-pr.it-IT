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
ms.openlocfilehash: 9b5765ff3c59b1312bead41a45a53478a96260df0567f006ab93c3ccfaf4be64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044344"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>Comportamento di ConsistencyGuid/sourceAnchor

Azure AD Connessione (versione 1.1.524.0 e successiva) ora facilita l'uso di msDS-ConsistencyGuid come attributo sourceAnchor. Quando si usa questa funzionalità, Azure AD Connessione automaticamente le regole di sincronizzazione per:
  
- Utilizzare msDS-ConsistencyGuid come attributo sourceAnchor per gli oggetti User. ObjectGUID viene utilizzato per altri tipi di oggetto.
    
- Per qualsiasi oggetto utente AD locale il cui attributo msDS-ConsistencyGuid non è popolato, Azure AD Connessione scrive il valore objectGUID nell'attributo msDS-ConsistencyGuid in Active Directory locale. Dopo aver popolato l'attributo msDS-ConsistencyGuid, Azure AD Connessione esporta l'oggetto in Azure AD.
    
 **Nota:** Una volta importato un oggetto AD locale in Azure AD Connessione (ovvero importato nello spazio connettore AD e proiettato nel Metaverse), non è più possibile modificarne il valore sourceAnchor. Per specificare il valore sourceAnchor per un determinato oggetto AD locale, configurare il relativo attributo msDS-ConsistencyGuid prima di importarlo in Azure AD Connessione. 
  
Per altre informazioni su SourceAnchor e ConsistencyGuid, fare riferimento a: [Azure AD Connessione: Concetti di progettazione](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

