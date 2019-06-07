---
title: Fornire agli utenti l'accesso a SharePoint e OneDrive
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: a689769dab24e12832ddc0937bc5ddc3d71dbee3
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/07/2019
ms.locfileid: "34759260"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a><span data-ttu-id="f46c8-102">Fornire agli utenti l'accesso a SharePoint e OneDrive</span><span class="sxs-lookup"><span data-stu-id="f46c8-102">Give users access to SharePoint and OneDrive</span></span>

<span data-ttu-id="f46c8-103">Questo problema si verifica più frequentemente quando un utente viene eliminato e ricreato con lo stesso nome dell'entità utente (UPN, User Principal Name).</span><span class="sxs-lookup"><span data-stu-id="f46c8-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="f46c8-104">Il nuovo account viene creato utilizzando un valore PUID (Passport Unique ID) diverso.</span><span class="sxs-lookup"><span data-stu-id="f46c8-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="f46c8-105">Quando l'utente tenta di accedere a una raccolta siti o ai propri OneDrive, l'utente ha un PUID non corretto.</span><span class="sxs-lookup"><span data-stu-id="f46c8-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="f46c8-106">Un secondo scenario implica la sincronizzazione della directory con un'unità organizzativa di Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f46c8-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="f46c8-107">Se gli utenti hanno già effettuato l'accesso a SharePoint e quindi vengono spostati in un'altra unità organizzativa e risincronizzati con SharePoint, potrebbero verificarsi questo problema.</span><span class="sxs-lookup"><span data-stu-id="f46c8-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="f46c8-108">Per risolvere il problema, è necessario ripristinare l'UPN originale con i passaggi descritti nell'articolo,[ripristinare un utente in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="f46c8-108">To resolve this issue you should restore the original UPN with the steps in the article,[Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="f46c8-109">Una volta completata questa operazione, è possibile verificare che l'utente disponga dei diritti di amministratore per il sito di OneDrive attenendosi alla procedura seguente per [aggiungere l'amministratore per l'OneDrive di un utente](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive) .</span><span class="sxs-lookup"><span data-stu-id="f46c8-109">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span></span>

<span data-ttu-id="f46c8-110">Per ulteriori informazioni sui livelli di autorizzazione, vedere l'articolo, informazioni sui [livelli di autorizzazione in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="f46c8-110">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
