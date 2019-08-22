---
title: Risoluzione dei problemi relativi ai messaggi di accesso negato
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 0a885e15d54c9337711f2528628789dfcb903264
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36503534"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="3fb4d-102">Risoluzione dei problemi relativi ai messaggi di accesso negato nell'interfaccia di amministrazione di SharePoint/OneDrive</span><span class="sxs-lookup"><span data-stu-id="3fb4d-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="3fb4d-103">Se si riceve un messaggio di accesso negato quando si tenta di accedere a un interfaccia di amministrazione di SharePoint/OneDrive, assicurarsi [di assegnare una licenza all'utente](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="3fb4d-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="3fb4d-104">Se l'utente dispone di una licenza, è necessario assicurarsi che sia [assegnato un ruolo di amministratore](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) che può accedere ai centri di amministrazione.</span><span class="sxs-lookup"><span data-stu-id="3fb4d-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="3fb4d-105">Questo problema può verificarsi anche quando un utente viene eliminato e ricreato con lo stesso nome dell'entità utente (UPN).</span><span class="sxs-lookup"><span data-stu-id="3fb4d-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="3fb4d-106">Il nuovo account viene creato utilizzando un valore PUID (Passport Unique ID) diverso.</span><span class="sxs-lookup"><span data-stu-id="3fb4d-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="3fb4d-107">Quando l'utente tenta di accedere a una raccolta siti o ai propri OneDrive, l'utente ha un PUID non corretto.</span><span class="sxs-lookup"><span data-stu-id="3fb4d-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="3fb4d-108">Un secondo scenario implica la sincronizzazione della directory con un'unità organizzativa di Active Directory.</span><span class="sxs-lookup"><span data-stu-id="3fb4d-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="3fb4d-109">Se gli utenti hanno già effettuato l'accesso a SharePoint e quindi vengono spostati in un'altra unità organizzativa e risincronizzati con SharePoint, potrebbero verificarsi questo problema.</span><span class="sxs-lookup"><span data-stu-id="3fb4d-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="3fb4d-110">Per risolvere il problema, è necessario ripristinare l'UPN originale con i passaggi descritti nell'articolo, [ripristinare un utente in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="3fb4d-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="3fb4d-111">Nota: se un'interfaccia di amministrazione di OneDrive o SharePoint non è disponibile per più utenti che in precedenza avevano accesso, potrebbe verificarsi un problema di servizio temporaneo.</span><span class="sxs-lookup"><span data-stu-id="3fb4d-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="3fb4d-112">[Controllare il dashboard dell'integrità dei servizi](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="3fb4d-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


