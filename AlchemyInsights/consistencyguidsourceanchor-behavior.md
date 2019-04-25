---
title: Comportamento di ConsistencyGuid/sourceAnchor
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: cb1b50792b07a1b3b69607bf2f6824141a15922f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32408112"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>Comportamento di ConsistencyGuid/sourceAnchor

Azure AD Connect (Version 1.1.524.0 e After) facilita ora l'utilizzo di msDS-ConsistencyGuid come attributo sourceAnchor. Quando si utilizza questa funzionalità, Azure AD Connect configura automaticamente le regole di sincronizzazione per:
  
- Utilizzare msDS-ConsistencyGuid come attributo sourceAnchor per gli oggetti utente. ObjectGUID viene utilizzato per altri tipi di oggetti.
    
- Per qualsiasi oggetto utente di Active Directory locale, il cui attributo msDS-ConsistencyGuid non è popolato, Azure AD Connect scrive il relativo valore di objectGUID nell'attributo msDS-ConsistencyGuid in attivo locale. Dopo che l'attributo msDS-ConsistencyGuid è stato popolato, Azure AD Connect esporta quindi l'oggetto in Azure AD.
    
 **Nota:** Dopo aver importato un oggetto Active Directory locale in Azure AD Connect (ovvero importato nello spazio del connettore AD e proiettato nel metaverse), non è più possibile modificarne il valore sourceAnchor. Per specificare il valore sourceAnchor per un determinato oggetto AD locale, configurare il relativo attributo msDS-ConsistencyGuid prima di essere importato in Azure AD Connect. 
  
Per ulteriori informazioni su SourceAnchor e ConsistencyGuid, vedere i seguenti: [Azure ad Connect: Concepts design](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

