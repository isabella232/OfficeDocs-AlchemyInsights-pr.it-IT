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
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="43f23-102">ConsistencyGuid / sourceAnchor comportamento</span><span class="sxs-lookup"><span data-stu-id="43f23-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="43f23-p101">Connetti Azure Active Directory (versione 1.1.524.0 e una volta eseguito) ora semplifica l'utilizzo dell'attributo msDS-ConsistencyGuid come attributo sourceAnchor. Quando si utilizza questa funzionalità, Connetti Azure Active Directory vengono configurate automaticamente le regole di sincronizzazione per:</span><span class="sxs-lookup"><span data-stu-id="43f23-p101">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute. When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="43f23-p102">Utilizzare msDS-ConsistencyGuid come l'attributo sourceAnchor per gli oggetti utente. ObjectGUID viene utilizzato per altri tipi di oggetto.</span><span class="sxs-lookup"><span data-stu-id="43f23-p102">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects. ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="43f23-p103">Per qualsiasi oggetto utente locale di Active Directory oggetto il cui attributo msDS-ConsistencyGuid non viene popolate, Azure scritture Connetti AD eseguire il relativo valore objectGUID nell'attributo msDS-ConsistencyGuid in Active Directory locale. Dopo che l'attributo msDS-ConsistencyGuid viene popolato, Azure Active Directory Connetti Esporta l'oggetto Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="43f23-p103">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory. After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="43f23-p104">**Nota:** Una volta un locale importazione di oggetti Active Directory in Azure Connect Active Directory (ovvero, importato nello spazio connettore Active Directory e stimare nel Metaverse), non è possibile modificare il relativo valore sourceAnchor diversi. Per specificare il valore sourceAnchor per un dato locale Active Directory dell'oggetto, configurare l'attributo msDS-ConsistencyGuid prima dell'importazione in Azure Active Directory Connetti.</span><span class="sxs-lookup"><span data-stu-id="43f23-p104">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore. To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="43f23-111">Per ulteriori informazioni su SourceAnchor e ConsistencyGuid, fare riferimento agli elementi seguenti: [Connetti Azure Active Directory: progettare concetti](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="43f23-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

