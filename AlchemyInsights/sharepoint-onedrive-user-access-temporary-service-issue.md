---
title: Problemi relativi alle prestazioni-SharePoint o OneDrive
ms.author: pebaum
author: pebaum
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 2db0a9442b9fdf1752b654f7c188e641e0a274cb
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053805"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="21406-102">SharePoint o OneDrive lento, inaccessibile o non disponibile per più utenti</span><span class="sxs-lookup"><span data-stu-id="21406-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="21406-103">Se un sito di OneDrive o di SharePoint non è disponibile per più utenti che in precedenza avevano accesso, potrebbe verificarsi un problema di servizio temporaneo.</span><span class="sxs-lookup"><span data-stu-id="21406-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="21406-104">[Controllare il dashboard dell'integrità dei servizi](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="21406-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="21406-105">**Aggiungere e concedere una licenza all'utente**</span><span class="sxs-lookup"><span data-stu-id="21406-105">**Add and license the user**</span></span>

<span data-ttu-id="21406-106">Assicurarsi [di assegnare licenze agli utenti in Office 365 for business](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="21406-106">Ensure that you [Assign licenses to users in Office 365 for business](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span>


<span data-ttu-id="21406-107">**Assegnare le autorizzazioni**</span><span class="sxs-lookup"><span data-stu-id="21406-107">**Assign Permissions**</span></span>

<span data-ttu-id="21406-108">Se all'utente è stata assegnata una licenza di SharePoint ed è ancora in ricezione un messaggio di accesso negato, assicurarsi che disponga del [livello di autorizzazione appropriato](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assegnato.</span><span class="sxs-lookup"><span data-stu-id="21406-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="21406-109">**Valutare la possibilità di utilizzare la funzionalità di richiesta di accesso**</span><span class="sxs-lookup"><span data-stu-id="21406-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="21406-110">La [funzionalità di richiesta di accesso](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) consente agli utenti di richiedere l'accesso ai contenuti che attualmente non dispongono dell'autorizzazione per la vista.</span><span class="sxs-lookup"><span data-stu-id="21406-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="21406-111">**Consenti lo script personalizzato può causare problemi di accesso negato**</span><span class="sxs-lookup"><span data-stu-id="21406-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="21406-112">Esistono alcuni scenari in cui la caratteristica *Consenti script personalizzato* potrebbe presentare un accesso negato.</span><span class="sxs-lookup"><span data-stu-id="21406-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="21406-113">Per un elenco delle caratteristiche coinvolte, considerazioni sulla sicurezza e la possibilità di disabilitare la funzionalità.</span><span class="sxs-lookup"><span data-stu-id="21406-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="21406-114">Visitare [Consenti o Impedisci lo script personalizzato](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="21406-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

