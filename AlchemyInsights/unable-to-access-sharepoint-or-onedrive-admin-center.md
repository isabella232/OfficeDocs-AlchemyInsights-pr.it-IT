---
title: Non è possibile accedere all'interfaccia di amministrazione di SharePoint o OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001459"
- "5638"
ms.openlocfilehash: a70b0708b325c5feaefec3d97c957086d7f62cc6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749482"
---
# <a name="unable-to-access-sharepoint-or-onedrive-admin-center"></a><span data-ttu-id="b1b16-102">Non è possibile accedere all'interfaccia di amministrazione di SharePoint o OneDrive</span><span class="sxs-lookup"><span data-stu-id="b1b16-102">Unable to access SharePoint or OneDrive admin center</span></span>

- <span data-ttu-id="b1b16-103">Se il sito dell'interfaccia di amministrazione di SharePoint o OneDrive non è accessibile o disponibile, è possibile che si sia verificato un problema temporaneo per cui gli utenti riscontrano ritardi intermittenti o errori di navigazione durante l'accesso ai siti di SharePoint o ai contenuti di OneDrive.</span><span class="sxs-lookup"><span data-stu-id="b1b16-103">If your SharePoint or OneDrive Admin center site is inaccessible or unavailable, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="b1b16-104">Controllare il [dashboard sull'integrità dei servizi](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) per verificare se l'organizzazione è interessata.</span><span class="sxs-lookup"><span data-stu-id="b1b16-104">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

- <span data-ttu-id="b1b16-105">Agli amministratori globali e di SharePoint è necessario assegnare una licenza di SharePoint.</span><span class="sxs-lookup"><span data-stu-id="b1b16-105">Global and SharePoint admins need to be assigned a SharePoint license.</span></span> <span data-ttu-id="b1b16-106">Gli account appena creati ai quali è stata appena assegnata una licenza o un ruolo di amministratore di SharePoint potrebbero riscontrare problemi di accesso a SharePoint, ad esempio di tipo "accesso negato" o "utente non trovato".</span><span class="sxs-lookup"><span data-stu-id="b1b16-106">Newly created accounts just assigned with a SharePoint License or Admin role might experience issues accessing SharePoint, like "access denied" or "user not found."</span></span> <span data-ttu-id="b1b16-107">Attendere almeno 24 ore per il completamento della sincronizzazione tra i sistemi.</span><span class="sxs-lookup"><span data-stu-id="b1b16-107">Please give at least 24 hours for sync to complete across our systems.</span></span> <span data-ttu-id="b1b16-108">Ci rendiamo conto che 24 ore può sembrare molto.</span><span class="sxs-lookup"><span data-stu-id="b1b16-108">We understand that 24 hours may seem like a long time.</span></span> <span data-ttu-id="b1b16-109">In molti casi, stiamo già lavorando a una soluzione.</span><span class="sxs-lookup"><span data-stu-id="b1b16-109">In many cases, we're already working on a solution.</span></span>

- <span data-ttu-id="b1b16-110">Gli utenti di Privileged Identity Management ([PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new)) potrebbero ricevere un messaggio di accesso negato se la finestra di tempo di accesso consentito è molto piccola, vedere [Accesso negato agli account PIM](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts).</span><span class="sxs-lookup"><span data-stu-id="b1b16-110">Privileged Identity Management ([PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new))  users may receive access denied if allowed access time window is very small, see  [Access denied to PIM accounts](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts).</span></span>