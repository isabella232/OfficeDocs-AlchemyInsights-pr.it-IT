---
title: Sincronizzazione dei servizi di dominio
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003245"
- "7922"
- "7921"
ms.openlocfilehash: b35d3a402bc08a27a818209385c5666b901fa524
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/15/2021
ms.locfileid: "49876517"
---
# <a name="domain-service-synchronization"></a><span data-ttu-id="0120d-102">Sincronizzazione dei servizi di dominio</span><span class="sxs-lookup"><span data-stu-id="0120d-102">Domain service synchronization</span></span>

<span data-ttu-id="0120d-103">Gli oggetti e le credenziali di un dominio gestito di Azure Active Directory (Azure AD DS) possono essere creati localmente all'interno del dominio oppure sincronizzati da un tenant di Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="0120d-103">Objects and credentials in an Azure Active Directory Domain Services (Azure AD DS) managed domain can either be created locally within the domain, or synchronized from an Azure Active Directory (Azure AD) tenant.</span></span> <span data-ttu-id="0120d-104">Quando si distribuisce Azure AD DS per la prima volta, viene configurata e avviata una sincronizzazione automatica unidirezionale per replicare gli oggetti da Azure AD.</span><span class="sxs-lookup"><span data-stu-id="0120d-104">When you first deploy Azure AD DS, an automatic one-way synchronization is configured and initiated to replicate the objects from Azure AD.</span></span> <span data-ttu-id="0120d-105">Questa sincronizzazione unidirezionale continua a essere eseguita in background per mantenere il dominio gestito di Azure AD DS aggiornato con le modifiche apportate da Azure AD.</span><span class="sxs-lookup"><span data-stu-id="0120d-105">This one-way synchronization continues to run in the background to keep the Azure AD DS managed domain up-to-date with any changes from Azure AD.</span></span> <span data-ttu-id="0120d-106">Nessuna sincronizzazione si verifica da Azure AD DS di nuovo ad Azure AD.</span><span class="sxs-lookup"><span data-stu-id="0120d-106">No synchronization occurs from Azure AD DS back to Azure AD.</span></span>

<span data-ttu-id="0120d-107">Per ulteriori informazioni sulla sincronizzazione dei servizi di dominio di Azure Active Directory, vedere [Domain Service Synchronization](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization).</span><span class="sxs-lookup"><span data-stu-id="0120d-107">For more details on Azure Active Directory domain service synchronization, see [Domain Service Synchronization](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization).</span></span> 
