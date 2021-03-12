---
title: Risoluzione dei problemi relativi ai messaggi di accesso negato
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3189fa61d28253569278024d4191ee63b917509f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707958"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="100a4-102">Risolvere i problemi relativi ai messaggi di accesso negato nell'interfaccia di amministrazione di Sharepoint/OneDrive</span><span class="sxs-lookup"><span data-stu-id="100a4-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="100a4-103">Se si riceve un messaggio di accesso negato quando si tenta di passare a un'interfaccia di amministrazione di Sharepoint/OneDrive, assicurarsi di assegnare una licenza [all'utente.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)</span><span class="sxs-lookup"><span data-stu-id="100a4-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="100a4-104">Se l'utente ha una licenza, è inoltre necessario assicurarsi che gli sia assegnato un ruolo [di](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) amministratore in grado di accedere alle centri di amministrazione.</span><span class="sxs-lookup"><span data-stu-id="100a4-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="100a4-105">Questo problema può verificarsi anche quando un utente viene eliminato e ri creato di nuovo con lo stesso nome dell'entità utente (UPN).</span><span class="sxs-lookup"><span data-stu-id="100a4-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="100a4-106">Il nuovo account viene creato utilizzando un valore PUID (ID univoco Passport) diverso.</span><span class="sxs-lookup"><span data-stu-id="100a4-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="100a4-107">Quando l'utente tenta di accedere a una raccolta siti o a OneDrive, l'utente ha un PUID non corretto.</span><span class="sxs-lookup"><span data-stu-id="100a4-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="100a4-108">Un secondo scenario prevede la sincronizzazione della directory con un'unità organizzativa (OU) di Active Directory.</span><span class="sxs-lookup"><span data-stu-id="100a4-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="100a4-109">Se gli utenti hanno già eseguito l'accesso a SharePoint e quindi vengono spostati in un'unità organizzativa diversa e sincronizzati nuovamente con SharePoint, è possibile che si verifichi questo problema.</span><span class="sxs-lookup"><span data-stu-id="100a4-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="100a4-110">Per risolvere questo problema, è consigliabile ripristinare l'UPN originale con la procedura descritta nell'articolo Ripristinare [un utente in Microsoft 365.](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)</span><span class="sxs-lookup"><span data-stu-id="100a4-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="100a4-111">Nota: se un'interfaccia di amministrazione di OneDrive o SharePoint non è disponibile per più utenti che hanno avuto accesso in precedenza, potrebbe verificarsi un problema di servizio temporaneo.</span><span class="sxs-lookup"><span data-stu-id="100a4-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="100a4-112">[Controllare il dashboard sull'integrità del servizio.](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="100a4-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


