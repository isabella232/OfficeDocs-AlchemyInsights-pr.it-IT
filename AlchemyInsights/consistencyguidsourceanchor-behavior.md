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
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="37138-102">Comportamento di ConsistencyGuid/sourceAnchor</span><span class="sxs-lookup"><span data-stu-id="37138-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="37138-103">Azure AD Connect (versione 1.1.524.0 e successiva) ora facilita l'uso di msDS-ConsistencyGuid come attributo sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="37138-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="37138-104">Quando si usa questa funzionalità, Azure AD Connect configura automaticamente le regole di sincronizzazione per:</span><span class="sxs-lookup"><span data-stu-id="37138-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="37138-105">Utilizzare msDS-ConsistencyGuid come attributo sourceAnchor per gli oggetti User.</span><span class="sxs-lookup"><span data-stu-id="37138-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="37138-106">ObjectGUID viene utilizzato per altri tipi di oggetto.</span><span class="sxs-lookup"><span data-stu-id="37138-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="37138-107">Per qualsiasi oggetto utente AD locale il cui attributo msDS-ConsistencyGuid non è popolato, Azure AD Connect scrive il valore objectGUID nell'attributo msDS-ConsistencyGuid in Active Directory locale.</span><span class="sxs-lookup"><span data-stu-id="37138-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="37138-108">Dopo aver popolato l'attributo msDS-ConsistencyGuid, Azure AD Connect esporta quindi l'oggetto in Azure AD.</span><span class="sxs-lookup"><span data-stu-id="37138-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="37138-109">**Nota:** Dopo l'importazione di un oggetto AD locale in Azure AD Connect, ovvero importato nello spazio connettore AD e proiettato nel Metaverse, non è più possibile modificarne il valore sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="37138-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="37138-110">Per specificare il valore sourceAnchor per un determinato oggetto AD locale, configurare il relativo attributo msDS-ConsistencyGuid prima di importarlo in Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="37138-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="37138-111">Per altre informazioni su SourceAnchor e ConsistencyGuid, fare riferimento a: [Azure AD Connect: Concetti di progettazione](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="37138-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

