---
title: Mapping degli attributi di provisioning degli utenti
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7851"
- "9004348"
ms.openlocfilehash: 8bbf554c533d960a304901d7cbb492b87e9bec71
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 01/22/2021
ms.locfileid: "49935365"
---
# <a name="user-provisioning-attribute-mapping"></a><span data-ttu-id="e50ed-102">Mapping degli attributi di provisioning degli utenti</span><span class="sxs-lookup"><span data-stu-id="e50ed-102">User-provisioning attribute mapping</span></span>

1. <span data-ttu-id="e50ed-103">Per la risoluzione dei problemi noti di mapping degli attributi, vedere [Mapping degli attributi](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings).</span><span class="sxs-lookup"><span data-stu-id="e50ed-103">To troubleshoot known attribute-mapping issues, see [Attribute mappings](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings).</span></span> 
2. <span data-ttu-id="e50ed-104">Microsoft Azure Active Directory (AD) fornisce supporto per il provisioning degli utenti ad applicazioni SaaS di terze parti, ad esempio Salesforce, G Suite e altri.</span><span class="sxs-lookup"><span data-stu-id="e50ed-104">Microsoft Azure Active Directory (AD) provides support for user provisioning to third-party SaaS applications such as Salesforce, G Suite and others.</span></span> <span data-ttu-id="e50ed-105">Se si abilita il provisioning degli utenti per un'applicazione SaaS di terze parti, il portale di Azure controlla i relativi valori degli attributi tramite mapping degli attributi.</span><span class="sxs-lookup"><span data-stu-id="e50ed-105">If you enable user provisioning for a third-party SaaS application, the Azure portal controls its attribute values through attribute-mappings.</span></span> <span data-ttu-id="e50ed-106">Per informazioni su come personalizzare i mapping degli attributi predefiniti, vedere [Personalizzare i mapping degli attributi di provisioning degli utenti per applicazioni SaaS in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).</span><span class="sxs-lookup"><span data-stu-id="e50ed-106">To learn how to customize the default attribute-mappings, see [Customize user provisioning attribute-mappings for SaaS applications in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).</span></span>
    - <span data-ttu-id="e50ed-107">Per altre informazioni sul provisioning degli utenti delle applicazioni SaaS, vedere [Cos'è il provisioning degli utenti per le app SaaS in Azure AD?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning).</span><span class="sxs-lookup"><span data-stu-id="e50ed-107">To learn more about SaaS app user provisioning, see [What is automated SaaS app user provisioning in Azure AD?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)</span></span> 
3. <span data-ttu-id="e50ed-108">Durante la personalizzazione del mapping attributi per il provisioning degli utenti, l'attributo per cui si desidera eseguire il mapping potrebbe non comparire nell'elenco attributi di origine.</span><span class="sxs-lookup"><span data-stu-id="e50ed-108">When customizing attribute-mappings for user provisioning, you might find that the attribute you want to map doesn't appear in the Source attribute list.</span></span> <span data-ttu-id="e50ed-109">L'articolo [Sincronizzare un attributo da Active Directory locale ad Azure AD per eseguire il provisioning di un'applicazione](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) mostra come aggiungere l'attributo mancante sincronizzandolo da Active Directory locale ad Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e50ed-109">The [Sync an attribute from your on-premises Active Directory to Azure AD for provisioning to an application](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) article shows you how to add the missing attribute by synchronizing it from your on-premises AD to Azure AD.</span></span>
