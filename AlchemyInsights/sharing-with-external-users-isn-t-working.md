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
ms.custom: Adm_O365
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 4b132a3cb0fac015ab44a1fa08565af15b7e8121
ms.sourcegitcommit: c003a5db7edc3a44fb5b31b46cd45f12b62d172a
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 02/22/2019
ms.locfileid: "30207689"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="a2c88-102">Risolvere i problemi di condivisione del contenuto di SharePoint con utenti esterni</span><span class="sxs-lookup"><span data-stu-id="a2c88-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="a2c88-103">Verificare che la condivisione esterna sia attivata per l'organizzazione:</span><span class="sxs-lookup"><span data-stu-id="a2c88-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="a2c88-104">Passare alla [pagina componenti &amp; aggiuntivi servizi nell'interfaccia di amministrazione di Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)e quindi fare clic su **siti**.</span><span class="sxs-lookup"><span data-stu-id="a2c88-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="a2c88-p101">Verificare che l'impostazione sia attivata su "attivo". Se è selezionata l'opzione "solo utenti esterni esistenti", verificare che l'utente esterno sia elencato nell'interfaccia di amministrazione di Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="a2c88-p101">Make sure the setting is turned to "On." If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="a2c88-p102">Assicurarsi che la condivisione esterna sia attivata per il sito. Per una raccolta siti classica:</span><span class="sxs-lookup"><span data-stu-id="a2c88-p102">Make sure external sharing it turned on for the site. For a classic site collection:</span></span>
  
1. <span data-ttu-id="a2c88-109">Nel riquadro sinistro dell'interfaccia di amministrazione di SharePoint classico fare clic su **raccolte siti**.</span><span class="sxs-lookup"><span data-stu-id="a2c88-109">In the classic SharePoint admin center, in the left pane, click **site collections**.</span></span>
    
2. <span data-ttu-id="a2c88-110">Selezionare il sito o i siti e sulla barra multifunzione fare clic su **condivisione**.</span><span class="sxs-lookup"><span data-stu-id="a2c88-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="a2c88-111">Per un sito del team che appartiene a un gruppo di Office 365 o a un sito di comunicazione:</span><span class="sxs-lookup"><span data-stu-id="a2c88-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="a2c88-p103">Questi nuovi tipi di sito hanno la stessa impostazione di condivisione dell'impostazione a livello di organizzazione, a meno che l'impostazione a livello di organizzazione non consenta la condivisione dei file tramite collegamenti che non richiedono l'accesso. In questo caso, i siti consentono la condivisione con utenti esterni nuovi ed esistenti che effettuano l'accesso. Per modificare l'impostazione per siti specifici, utilizzare la nuova interfaccia di amministrazione di SharePoint (anteprima) o PowerShell. Per ulteriori [informazioni](https://go.microsoft.com/fwlink/?linkid=871863), vedere.</span><span class="sxs-lookup"><span data-stu-id="a2c88-p103">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in. In this case, the sites allow sharing with new and existing external users who sign in. To change the setting for specific sites, use the new SharePoint admin center (preview) or PowerShell. [Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="a2c88-116">L'impostazione di condivisione esterna per qualsiasi sito può essere più restrittiva rispetto all'impostazione a livello dell'organizzazione, ma non più permissiva rispetto all'impostazione a livello dell'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="a2c88-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

