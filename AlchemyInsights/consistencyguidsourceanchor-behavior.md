---
title: ConsistencyGuid / sourceAnchor comportamento
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: e1ffa9cf2b59570cb6ea3517efad7a55fd9489a8
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29927659"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid / sourceAnchor comportamento

Connetti Azure Active Directory (versione 1.1.524.0 e una volta eseguito) ora semplifica l'utilizzo dell'attributo msDS-ConsistencyGuid come attributo sourceAnchor. Quando si utilizza questa funzionalità, Connetti Azure Active Directory vengono configurate automaticamente le regole di sincronizzazione per:
  
- Utilizzare msDS-ConsistencyGuid come l'attributo sourceAnchor per gli oggetti utente. ObjectGUID viene utilizzato per altri tipi di oggetto.
    
- Per qualsiasi oggetto utente locale di Active Directory oggetto il cui attributo msDS-ConsistencyGuid non viene popolate, Azure scritture Connetti AD eseguire il relativo valore objectGUID nell'attributo msDS-ConsistencyGuid in Active Directory locale. Dopo che l'attributo msDS-ConsistencyGuid viene popolato, Azure Active Directory Connetti Esporta l'oggetto Azure Active Directory.
    
 **Nota:** Una volta un locale importazione di oggetti Active Directory in Azure Connect Active Directory (ovvero, importato nello spazio connettore Active Directory e stimare nel Metaverse), non è possibile modificare il relativo valore sourceAnchor diversi. Per specificare il valore sourceAnchor per un dato locale Active Directory dell'oggetto, configurare l'attributo msDS-ConsistencyGuid prima dell'importazione in Azure Active Directory Connetti. 
  
Per ulteriori informazioni su SourceAnchor e ConsistencyGuid, fare riferimento agli elementi seguenti: [Connetti Azure Active Directory: progettare concetti](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

