---
title: Problemi con la licenza di Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: f0a7625c7b77860e5ba0e29f2df47101749aace3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47657280"
---
# <a name="yammer-licensing-issues"></a><span data-ttu-id="c1a9f-102">Problemi con la licenza di Yammer</span><span class="sxs-lookup"><span data-stu-id="c1a9f-102">Yammer licensing issues</span></span>

<span data-ttu-id="c1a9f-103">Tutti gli utenti devono disporre di una licenza per usare il servizio Yammer Enterprise, ma per impostazione predefinita, Yammer non richiede che gli utenti abbiano una licenza per accedere al servizio.</span><span class="sxs-lookup"><span data-stu-id="c1a9f-103">All users must have a license to use the Yammer Enterprise service, but by default Yammer does not require that users have a license to access the service.</span></span> <span data-ttu-id="c1a9f-104">Quando un amministratore modifica l'impostazione per bloccare gli utenti di Microsoft 365 senza licenza di Yammer, gli utenti a cui non sia stata assegnata una licenza di Yammer Enterprise non possono accedere al servizio Yammer.</span><span class="sxs-lookup"><span data-stu-id="c1a9f-104">When an administrator changes the setting to block Microsoft 365 users without Yammer licenses, users not assigned a Yammer Enterprise license can't access the Yammer service.</span></span> <span data-ttu-id="c1a9f-105">Per ulteriori informazioni, vedere [Gestire le licenze utente di Yammer in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="c1a9f-105">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span></span> 

<span data-ttu-id="c1a9f-106">Quando le licenze vengono rimosse dagli utenti, il riquadro Yammer non viene più visualizzato e altri servizi possono usare la rimozione della licenza per nascondere le funzionalità.</span><span class="sxs-lookup"><span data-stu-id="c1a9f-106">When licenses are removed from users, the Yammer tile is no longer displayed, and other services can use license removal to hide features.</span></span> <span data-ttu-id="c1a9f-107">In altri casi, le funzionalità possono comunque essere visualizzate, ma è necessario assegnare delle licenze per poterle utilizzare.</span><span class="sxs-lookup"><span data-stu-id="c1a9f-107">In other cases, features can still appear but require licence assignment to operate.</span></span>  

<span data-ttu-id="c1a9f-108">**La licenza non viene aggiornata per l'utente**</span><span class="sxs-lookup"><span data-stu-id="c1a9f-108">**License is not getting updated for the user**</span></span>  

<span data-ttu-id="c1a9f-109">A volte, a un utente è assegnata una licenza, ma non è ancora possibile accedere a Yammer.</span><span class="sxs-lookup"><span data-stu-id="c1a9f-109">Occasionally, a user is assigned a license but is still unable to access Yammer.</span></span> <span data-ttu-id="c1a9f-110">È più probabile che si verifichino ritardi quando è in corso un'assegnazione di licenza in blocco.</span><span class="sxs-lookup"><span data-stu-id="c1a9f-110">Delays are more likely to occur when a mass license assignment is in progress.</span></span> <span data-ttu-id="c1a9f-111">Gli utenti di Yammer potrebbero non essere aggiornati nello stesso ordine in cui le licenze sono state modificate in Azure AD perché il sistema viene eseguito in modo asincrono.</span><span class="sxs-lookup"><span data-stu-id="c1a9f-111">Yammer users might not be updated in the same order as licenses are changed in Azure AD because the system runs asynchronously.</span></span> <span data-ttu-id="c1a9f-112">Attendere fino a 24 ore prima di aprire un caso di supporto per segnalare i problemi di sincronizzazione della licenza.</span><span class="sxs-lookup"><span data-stu-id="c1a9f-112">Wait up to 24 hours before opening a support case to report license sync issues.</span></span>  

<span data-ttu-id="c1a9f-113">**Assegnazione di licenze in blocco**</span><span class="sxs-lookup"><span data-stu-id="c1a9f-113">**Bulk licence assignment**</span></span>  

<span data-ttu-id="c1a9f-114">È possibile assegnare licenze tramite l'interfaccia di amministrazione o gli script di PowerShell.</span><span class="sxs-lookup"><span data-stu-id="c1a9f-114">Licenses can be assigned through the admin center or PowerShell scripting.</span></span> <span data-ttu-id="c1a9f-115">Per altre informazioni, vedere [Assegnare licenze agli utenti](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) e [Assegnare licenze agli account utente con Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span><span class="sxs-lookup"><span data-stu-id="c1a9f-115">For more info, see [Assign licenses to users](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) and [Assign licenses to user accounts with Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span></span> 

<span data-ttu-id="c1a9f-116">Il supporto Microsoft non offre assistenza per la creazione di script, ma è disponibile la documentazione sull'assegnazione di licenze di Yammer.</span><span class="sxs-lookup"><span data-stu-id="c1a9f-116">Microsoft Support does not provide assistance with creating scripts, but documentation on Yammer license assignment is available.</span></span> <span data-ttu-id="c1a9f-117">Per altre informazioni, vedere [Gestire le licenze di Yammer usando Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span><span class="sxs-lookup"><span data-stu-id="c1a9f-117">For more info, see [Manage Yammer licenses by using Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span></span>