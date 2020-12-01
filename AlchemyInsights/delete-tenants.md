---
title: Elimina tenant
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/30/2020
ms.locfileid: "49477675"
---
# <a name="delete-tenant"></a><span data-ttu-id="fe420-102">Elimina tenant</span><span class="sxs-lookup"><span data-stu-id="fe420-102">Delete tenant</span></span>

<span data-ttu-id="fe420-103">Per eliminare un annuncio di Azure, verificare quanto segue:</span><span class="sxs-lookup"><span data-stu-id="fe420-103">To delete an Azure AD, ensure:</span></span>
- <span data-ttu-id="fe420-104">Si è un amministratore globale nella directory.</span><span class="sxs-lookup"><span data-stu-id="fe420-104">You are a Global Administrator on the directory.</span></span>
- <span data-ttu-id="fe420-105">L'utente non ha eseguito l'accesso con un account che include la directory predefinita, ad esempio contoso.onmicrosoft.com, nell'account signed-in, ad esempio admin@contoso.onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="fe420-105">You are NOT signed in with an account that has the default directory such as contoso.onmicrosoft.com in the signed--in account, such as admin@contoso.onmicrosoft.com.</span></span>
- <span data-ttu-id="fe420-106">Rimuovere tutte le applicazioni attive nella directory prima dell'eliminazione.</span><span class="sxs-lookup"><span data-stu-id="fe420-106">Remove any active applications in the directory before deletion.</span></span> <span data-ttu-id="fe420-107">Per rimuovere le applicazioni attive, passare a registrazioni delle app e rimuovere le applicazioni esistenti.</span><span class="sxs-lookup"><span data-stu-id="fe420-107">To remove active applications, navigate to App registrations and remove the existing applications.</span></span>
- <span data-ttu-id="fe420-108">Non vi sono abbonamenti attivi per i Microsoft Online Services, ad esempio Microsoft Azure, Office 365 o Azure AD Premium associati alla directory.</span><span class="sxs-lookup"><span data-stu-id="fe420-108">There are no active subscriptions for any Microsoft Online Services, such as Microsoft Azure, Office 365 or Azure AD Premium associated on the directory.</span></span> <span data-ttu-id="fe420-109">Trasferire gli abbonamenti o velocizzare l'annullamento di abbonamenti attivi tramite il supporto e la fatturazione di Azure.</span><span class="sxs-lookup"><span data-stu-id="fe420-109">Transfer your subscriptions or expedite cancellation of active subscriptions via Azure Support and Billing.</span></span> <span data-ttu-id="fe420-110">Per ulteriori informazioni, vedere Annullamento delle sottoscrizioni di Office 365 e Azure.</span><span class="sxs-lookup"><span data-stu-id="fe420-110">Learn more on How to Cancel Office 365 and Azure subscriptions.</span></span> <span data-ttu-id="fe420-111">Per informazioni sull'associazione o l'aggiunta di una sottoscrizione esistente a un tenant, vedere [associare o aggiungere una sottoscrizione di Azure al tenant di Azure ad](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span><span class="sxs-lookup"><span data-stu-id="fe420-111">For guidance on associating or adding an existing subscription to a tenant, see [Associate or add an Azure subscription to your Azure AD tenant](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span></span>
- <span data-ttu-id="fe420-112">Non sono disponibili licenze attive.</span><span class="sxs-lookup"><span data-stu-id="fe420-112">There are no Active license.</span></span> <span data-ttu-id="fe420-113">Per rimuovere le licenze, vedere [come rimuovere la sottoscrizione per rimuovere la licenza](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).</span><span class="sxs-lookup"><span data-stu-id="fe420-113">To remove licenses, see [How to remove Subscription to Remove license](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).</span></span>
- <span data-ttu-id="fe420-114">Non ci sono altri utenti attivi nella directory oltre all'amministratore globale quando si tenta di eliminare l'Azure AD.</span><span class="sxs-lookup"><span data-stu-id="fe420-114">There are no other active users in the directory besides yourself as the Global Administrator when attempting to delete the Azure AD.</span></span> <span data-ttu-id="fe420-115">Rimuovere qualsiasi altro utente attivo e devono essere rimosse anche eventuali dipendenze su un nome di dominio personalizzato nel tenant, ad esempio gli utenti creati con admin@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="fe420-115">Remove any other active users, and any dependencies on a custom domain name in the tenant will also need to be removed, such as users created with admin@contoso.com.</span></span>

<span data-ttu-id="fe420-116">Per ulteriori informazioni su come eseguire le operazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="fe420-116">For more detail steps on how to:</span></span>
- <span data-ttu-id="fe420-117">Eliminare "Azure Active Directory" o "sottoscrizione", vedere [Delete Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span><span class="sxs-lookup"><span data-stu-id="fe420-117">Delete "Azure Active Directory" or "subscription",  see [Delete Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span></span>
- <span data-ttu-id="fe420-118">Rimozione di applicazioni nella directory, vedere [rimozione di applicazioni](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span><span class="sxs-lookup"><span data-stu-id="fe420-118">Removing applications in the directory, see [Removing Applications](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span></span> 
