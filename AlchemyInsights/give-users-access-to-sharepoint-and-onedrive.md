---
title: Fornire agli utenti l'accesso a SharePoint e OneDrive
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
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: a7e9c0b7ffa5c11a2e24ee5fda6491f049f985f1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677211"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a><span data-ttu-id="2db97-102">Fornire agli utenti l'accesso a SharePoint e OneDrive</span><span class="sxs-lookup"><span data-stu-id="2db97-102">Give users access to SharePoint and OneDrive</span></span>

> [!NOTE]
> <span data-ttu-id="2db97-103">Se un sito di OneDrive o di SharePoint non è disponibile per più utenti che in precedenza avevano accesso, potrebbe verificarsi un problema di servizio temporaneo.</span><span class="sxs-lookup"><span data-stu-id="2db97-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> [<span data-ttu-id="2db97-104">Controllare il dashboard dell'integrità del servizio</span><span class="sxs-lookup"><span data-stu-id="2db97-104">Check the service health dashboard</span></span>](https://portal.office.com/adminportal/home#/servicehealth)
  
<span data-ttu-id="2db97-105">Se si desidera che gli utenti dell'organizzazione siano in grado di accedere e utilizzare SharePoint e OneDrive, è necessario aggiungere account per loro e assicurarsi che dispongano di una licenza che conferisca loro l'accesso a SharePoint e OneDrive.</span><span class="sxs-lookup"><span data-stu-id="2db97-105">If you want people in your organization to be able to sign in and use SharePoint and OneDrive, you need to add accounts for them and make sure they have a license that gives them access to SharePoint and OneDrive.</span></span> <span data-ttu-id="2db97-106">Il modo più semplice per aggiungere gli utenti è nell'interfaccia di amministrazione di Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="2db97-106">The easiest way to add users is in the Microsoft 365 admin center.</span></span>
  
1. <span data-ttu-id="2db97-107">Passare alla [pagina utenti attivi nell'interfaccia di amministrazione di Microsoft 365](https://portal.office.com/adminportal/home#/users)e quindi fare clic su **Aggiungi utente**.</span><span class="sxs-lookup"><span data-stu-id="2db97-107">Go to the [Active users page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/users), and then click **Add a user**.</span></span>
    
2. <span data-ttu-id="2db97-108">Inserire le informazioni per l'utente e verificare che in **licenze di prodotto**sia stata assegnata una licenza e che sia selezionato **SharePoint Online** .</span><span class="sxs-lookup"><span data-stu-id="2db97-108">Fill in the information for the user, and make sure that under **Product licenses**, a license is assigned and **SharePoint Online** is selected.</span></span> 
    
<span data-ttu-id="2db97-109">Si noti che se si consente la condivisione esterna nell'organizzazione, gli utenti possono condividere i contenuti di SharePoint e OneDrive con utenti esterni all'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="2db97-109">Note that if you allow external sharing in your organization, users can share SharePoint and OneDrive content with people outside the organization.</span></span> <span data-ttu-id="2db97-110">Non è necessario assegnare le licenze agli utenti esterni.</span><span class="sxs-lookup"><span data-stu-id="2db97-110">You don't need to give these external users licenses.</span></span> <span data-ttu-id="2db97-111">Non è inoltre necessario aggiungere account per loro, a meno che la condivisione non sia impostata su "solo utenti esterni esistenti".</span><span class="sxs-lookup"><span data-stu-id="2db97-111">You also don't need to add accounts for them, unless sharing is set to "Only existing external users."</span></span> <span data-ttu-id="2db97-112">In tal caso, se le persone non sono presenti nella directory dell'organizzazione, è necessario aggiungerle come utenti guest nell'interfaccia di amministrazione di Azure AD.</span><span class="sxs-lookup"><span data-stu-id="2db97-112">In that case, if the people aren't in your organization's directory, you need to add them as guest users in the Azure AD admin center.</span></span>
  

