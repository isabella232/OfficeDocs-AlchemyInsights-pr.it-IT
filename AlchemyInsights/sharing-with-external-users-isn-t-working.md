---
title: Condivisione con utenti esterni non funziona
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 305b3891e6c83e27b5c55c13757640e6e9d51a81
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/24/2019
ms.locfileid: "29475760"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="38666-102">Correggere i problemi con la condivisione di contenuto di SharePoint con utenti esterni</span><span class="sxs-lookup"><span data-stu-id="38666-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="38666-103">Verificare che condivisione esterna è attivata per l'organizzazione:</span><span class="sxs-lookup"><span data-stu-id="38666-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="38666-104">Visitare il [servizi &amp; pagina di componenti aggiuntivi nell'interfaccia di amministrazione di Office 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), fare clic su **siti**.</span><span class="sxs-lookup"><span data-stu-id="38666-104">Go to the [Services &amp; add-ins page in the Office 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="38666-p101">Verificare che l'impostazione è attivata per "In". Se sono selezionati "Solo esistenti gli utenti esterni", verificare che l'utente esterno sia presente nell'interfaccia di amministrazione di Office 365.</span><span class="sxs-lookup"><span data-stu-id="38666-p101">Make sure the setting is turned to "On." If "Only existing external users" is selected, make sure the external user is listed in the Office 365 admin center.</span></span>
    
<span data-ttu-id="38666-p102">Verificare che l'esterno condividerla attivato per il sito. Per una raccolta siti classica:</span><span class="sxs-lookup"><span data-stu-id="38666-p102">Make sure external sharing it turned on for the site. For a classic site collection:</span></span>
  
1. <span data-ttu-id="38666-109">Nell'interfaccia di amministrazione SharePoint classica, nel riquadro sinistro fare clic su **raccolte siti**.</span><span class="sxs-lookup"><span data-stu-id="38666-109">In the classic SharePoint admin center, in the left pane, click **site collections**.</span></span>
    
2. <span data-ttu-id="38666-110">Selezionare uno o più siti e sulla barra multifunzione fare clic su **condivisione**.</span><span class="sxs-lookup"><span data-stu-id="38666-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="38666-111">Per un sito del team che appartiene a un gruppo di Office 365, o un sito di comunicazione:</span><span class="sxs-lookup"><span data-stu-id="38666-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="38666-p103">Questi nuovi tipi di sito hanno la stessa impostazione condivisione impostazione sul livello di organizzazione, a meno che l'impostazione del livello di organizzazione consente la condivisione file mediante collegamenti che non richiedono l'accesso. In questo caso, i siti di consentono la condivisione con nuovi ed esistenti gli utenti esterni che effettuano l'accesso. Per modificare l'impostazione per specifici siti, utilizzare la nuova interfaccia di amministrazione di SharePoint (anteprima) o PowerShell. [Ulteriori informazioni](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="38666-p103">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in. In this case, the sites allow sharing with new and existing external users who sign in. To change the setting for specific sites, use the new SharePoint admin center (preview) or PowerShell. [Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="38666-116">L'impostazione della condivisione esterna per qualsiasi sito può essere più restrittivo dell'impostazione a livello di organizzazione, ma non più ampio di impostazione a livello di organizzazione.</span><span class="sxs-lookup"><span data-stu-id="38666-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

