---
title: Sincronizzazione dei gruppi
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8304"
- "9003234"
ms.openlocfilehash: 52c19b6dcc79968150a188b389c5481c122f7945
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 02/15/2021
ms.locfileid: "50243925"
---
# <a name="group-sync"></a><span data-ttu-id="cf88a-102">Sincronizzazione dei gruppi</span><span class="sxs-lookup"><span data-stu-id="cf88a-102">Group sync</span></span>

<span data-ttu-id="cf88a-103">Questo articolo fornisce indicazioni per la sincronizzazione dei gruppi.</span><span class="sxs-lookup"><span data-stu-id="cf88a-103">This article provides guidance on group synchronization.</span></span>

1. <span data-ttu-id="cf88a-104">Se un amministratore globale o un proprietario di gruppo non riesce a modificare le proprietà del gruppo, ad aggiungere membri o ad assegnare proprietari nel portale di Azure, assicurarsi che l'origine dell'autorità per il gruppo sia Azure Active Directory (Azure AD) per consentire all'amministratore globale o al proprietario di modificare il gruppo.</span><span class="sxs-lookup"><span data-stu-id="cf88a-104">If a global admin or group owner is not able to modify group properties or add members or assign owners in the Azure portal, ensure the source of the authority for the group is Azure Active Directory (Azure AD) for the global admin or group owner to modify the group.</span></span>
2. <span data-ttu-id="cf88a-105">Prima di provare a eliminare un gruppo sincronizzato in Azure AD, assicurarsi di aver [eliminato tutte le licenze assegnate](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced) per evitare errori.</span><span class="sxs-lookup"><span data-stu-id="cf88a-105">Before attempting to delete a synced group in Azure AD, ensure you have [deleted all assigned licenses](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced) to avoid errors.</span></span>

<span data-ttu-id="cf88a-106">Per informazioni su come sincronizzare utenti, gruppi e contatti, vedere [Sincronizzazione di Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts) e seguire le indicazioni dell'articolo [Sincronizzazione di un gruppo locale in Azure con Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) per sincronizzare gruppi locali con Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="cf88a-106">For understanding how to sync users, groups and contacts, see [Azure AD Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts), and follow [Syncing an on-premises group to Azure using Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) to sync on-perm groups using AD connect.</span></span>

<span data-ttu-id="cf88a-107">Vedere la guida [Risoluzione dei problemi relativi agli errori di sincronizzazione](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) per risolvere i problemi comuni che si verificano durante la sincronizzazione.</span><span class="sxs-lookup"><span data-stu-id="cf88a-107">Follow this guide [Troubleshooting Errors during synchronization](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) to troubleshoot common errors during synchronization.</span></span>

