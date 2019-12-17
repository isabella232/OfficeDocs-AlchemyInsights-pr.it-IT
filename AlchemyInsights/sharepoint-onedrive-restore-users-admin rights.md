---
title: Risoluzione dei problemi relativi ai messaggi di accesso negato ai siti di OneDrive for business
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9d8aba4e53a1e0505a430296bb1c11713ea2ce7b
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051609"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="4deb8-102">Risoluzione dei problemi relativi ai messaggi di accesso negato ai siti di OneDrive for business</span><span class="sxs-lookup"><span data-stu-id="4deb8-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="4deb8-103">Questo problema si verifica più frequentemente quando un utente viene eliminato e ricreato con lo stesso nome dell'entità utente (UPN, User Principal Name).</span><span class="sxs-lookup"><span data-stu-id="4deb8-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="4deb8-104">Il nuovo account viene creato utilizzando un valore PUID (Passport Unique ID) diverso.</span><span class="sxs-lookup"><span data-stu-id="4deb8-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="4deb8-105">Quando l'utente tenta di accedere a una raccolta siti o ai propri OneDrive, l'utente ha un PUID non corretto.</span><span class="sxs-lookup"><span data-stu-id="4deb8-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="4deb8-106">Un secondo scenario implica la sincronizzazione della directory con un'unità organizzativa di Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4deb8-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="4deb8-107">Se gli utenti hanno già effettuato l'accesso a SharePoint e quindi vengono spostati in un'altra unità organizzativa e risincronizzati con SharePoint, potrebbero verificarsi questo problema.</span><span class="sxs-lookup"><span data-stu-id="4deb8-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="4deb8-108">Per risolvere il problema, è necessario ripristinare l'UPN originale con i passaggi descritti nell'articolo, [ripristinare un utente in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="4deb8-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>
2. <span data-ttu-id="4deb8-109">Se non è possibile ripristinare l'utente originale, è necessario rimuovere l'utente precedente dal sito di OneDrive utilizzando questi passaggi, [rimuovere un utente dall'elenco informazioni utente]().</span><span class="sxs-lookup"><span data-stu-id="4deb8-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="4deb8-110">Una volta completata questa operazione, è possibile verificare che l'utente disponga dei diritti di amministratore per il sito di OneDrive attenendosi alla procedura seguente per [aggiungere l'amministratore per l'OneDrive di un utente](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive) .</span><span class="sxs-lookup"><span data-stu-id="4deb8-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span></span>

<span data-ttu-id="4deb8-111">Per ulteriori informazioni sui livelli di autorizzazione, vedere l'articolo, informazioni sui [livelli di autorizzazione in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="4deb8-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
