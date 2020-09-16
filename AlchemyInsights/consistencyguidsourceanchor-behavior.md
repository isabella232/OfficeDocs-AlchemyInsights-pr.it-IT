---
title: Comportamento di ConsistencyGuid/sourceAnchor
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: adac469328485696d1ee1532aa3d6828af0642eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47756287"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="9a666-102">Comportamento di ConsistencyGuid/sourceAnchor</span><span class="sxs-lookup"><span data-stu-id="9a666-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="9a666-103">Azure AD Connect (Version 1.1.524.0 e After) facilita ora l'utilizzo di msDS-ConsistencyGuid come attributo sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="9a666-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="9a666-104">Quando si utilizza questa funzionalità, Azure AD Connect configura automaticamente le regole di sincronizzazione per:</span><span class="sxs-lookup"><span data-stu-id="9a666-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="9a666-105">Utilizzare msDS-ConsistencyGuid come attributo sourceAnchor per gli oggetti utente.</span><span class="sxs-lookup"><span data-stu-id="9a666-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="9a666-106">ObjectGUID viene utilizzato per altri tipi di oggetti.</span><span class="sxs-lookup"><span data-stu-id="9a666-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="9a666-107">Per qualsiasi oggetto utente di Active Directory locale, il cui attributo msDS-ConsistencyGuid non è popolato, Azure AD Connect scrive il relativo valore di objectGUID nell'attributo msDS-ConsistencyGuid in attivo locale.</span><span class="sxs-lookup"><span data-stu-id="9a666-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="9a666-108">Dopo che l'attributo msDS-ConsistencyGuid è stato popolato, Azure AD Connect esporta quindi l'oggetto in Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9a666-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="9a666-109">**Nota:** Dopo aver importato un oggetto Active Directory locale in Azure AD Connect (ovvero importato nello spazio del connettore AD e proiettato nel metaverse), non è più possibile modificarne il valore sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="9a666-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="9a666-110">Per specificare il valore sourceAnchor per un determinato oggetto AD locale, configurare il relativo attributo msDS-ConsistencyGuid prima di essere importato in Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="9a666-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="9a666-111">Per ulteriori informazioni su SourceAnchor e ConsistencyGuid, vedere i seguenti: [Azure ad Connect: Concepts design](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="9a666-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

