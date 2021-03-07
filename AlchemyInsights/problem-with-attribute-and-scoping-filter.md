---
title: Problema con l'attributo e il filtro di ambito
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8470"
- "9004687"
ms.openlocfilehash: 78df24c0d8a670d678e26879cf81476f1ae9b92d
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430752"
---
# <a name="problem-with-attribute-and-scoping-filter"></a><span data-ttu-id="6c8ed-102">Problema con l'attributo e il filtro di ambito</span><span class="sxs-lookup"><span data-stu-id="6c8ed-102">Problem with attribute and scoping filter</span></span>

<span data-ttu-id="6c8ed-103">**Problema con valori UPN in conflitto**</span><span class="sxs-lookup"><span data-stu-id="6c8ed-103">**Issue with conflicting UPN values**</span></span>

<span data-ttu-id="6c8ed-104">Il provisioning utenti da Workday ad AD restituisce il messaggio di errore **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**.</span><span class="sxs-lookup"><span data-stu-id="6c8ed-104">The Workday to AD User Provisioning Workday to AD User Provisioning shows error message **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**.</span></span> <span data-ttu-id="6c8ed-105">L'operazione non è riuscita perché il valore UPN fornito per l'aggiunta o la modifica non è univoco a livello di foresta.</span><span class="sxs-lookup"><span data-stu-id="6c8ed-105">The operation failed because UPN value provided for addition/modification is not unique forest-wide.</span></span> <span data-ttu-id="6c8ed-106">Dettagli errore: **CONSTRAINT_ATT_TYPE - userPrincipalName**.</span><span class="sxs-lookup"><span data-stu-id="6c8ed-106">Error Details: **CONSTRAINT_ATT_TYPE - userPrincipalName**.</span></span>

<span data-ttu-id="6c8ed-107">Il valore **userPrincipalName** che il connettore Workday sta provando a impostare durante la creazione l'account utente di AD esiste già nel dominio Active Directory di destinazione.</span><span class="sxs-lookup"><span data-stu-id="6c8ed-107">The **userPrincipalName** value that Workday connector is trying to set when creating the AD user account already exists in the target AD domain.</span></span> <span data-ttu-id="6c8ed-108">Ciò significa che (1) l'utente esiste già e il controllo degli ID corrispondenti non è riuscito oppure (2) la regola di generazione UPN ha generato un valore in conflitto.</span><span class="sxs-lookup"><span data-stu-id="6c8ed-108">This implies that either (1) the user already exists and the matching ID check failed for the user or (2) the UPN generation rule generated a conflicting value.</span></span>

<span data-ttu-id="6c8ed-109">Ecco la procedura di risoluzione suggerita:</span><span class="sxs-lookup"><span data-stu-id="6c8ed-109">Here are the suggested resolution steps:</span></span>

<span data-ttu-id="6c8ed-110">Se l'utente esiste già e il controllo degli ID corrispondenti non è riuscito a collegare l'account Workday all'account Active Directory, verificare se l'attributo ID corrispondente ( in genere **employeeID**) sia in Workday che AD abbia una corrispondenza esatta.</span><span class="sxs-lookup"><span data-stu-id="6c8ed-110">If the user already exists and the matching ID check failed to link the Workday account to Active Directory account, then check if the matching ID attribute (typically **employeeID**) in both Workday and AD have an exact match.</span></span> <span data-ttu-id="6c8ed-111">Se non hanno corrispondenze, occorre risolvere un problema relativo ai dati.</span><span class="sxs-lookup"><span data-stu-id="6c8ed-111">If they don't have a match, it is a data issue that needs to be fixed.</span></span> <span data-ttu-id="6c8ed-112">Ad esempio, se l'EmployeeID in Workday è 001052 e in Active Directory è 1052, il motore di provisioning non riuscirà a collegare i due account e tenterà di creare un utente già esistente.</span><span class="sxs-lookup"><span data-stu-id="6c8ed-112">For example, if the EmployeeID in Workday is 001052 and in AD it is 1052, then the provisioning engine will fail to link the two accounts and will try to create a user that already exists.</span></span> <span data-ttu-id="6c8ed-113">La soluzione in questo caso consiste nel modificare il valore di **EmployeeID** in Active Directory in modo da includere gli zeri iniziali per impostarlo come 001052.</span><span class="sxs-lookup"><span data-stu-id="6c8ed-113">The solution in this case is to change the **EmployeeID** value in AD to include the leading zeros to make it 001052.</span></span>
<span data-ttu-id="6c8ed-114">Se l'espressione che genera l'UPN non genera un valore univoco, è consigliabile usare la funzione di deduplicazione **SelectUniqueValue** per generare un valore univoco ogni volta.</span><span class="sxs-lookup"><span data-stu-id="6c8ed-114">If the UPN-generating expression is not generating a unique value, consider using the de-duplication function **SelectUniqueValue** to generate a unique value each time.</span></span>

<span data-ttu-id="6c8ed-115">**Il provisioning utente da Workday ad AD non imposta il valore dell'attributo manager per l'account utente di AD**</span><span class="sxs-lookup"><span data-stu-id="6c8ed-115">**Workday to AD User Provisioning does not set manager attribute value for AD user account**</span></span>

<span data-ttu-id="6c8ed-116">Il provisioning utenti da Workday ad AD non imposta il valore dell'attributo **manager** per gli account utente di AD.</span><span class="sxs-lookup"><span data-stu-id="6c8ed-116">The Workday to AD User Provisioning job is not setting the **manager** attribute value for AD user accounts.</span></span> <span data-ttu-id="6c8ed-117">Questo comportamento può essere visualizzato in due scenari:</span><span class="sxs-lookup"><span data-stu-id="6c8ed-117">There are two possible scenarios when this behavior is seen:</span></span>

1. <span data-ttu-id="6c8ed-118">Il manager in Workday non può essere risolto in un account utente di AD corrispondente perché il manager non è nell'ambito.</span><span class="sxs-lookup"><span data-stu-id="6c8ed-118">The manager in Workday cannot be resolved to a corresponding AD User account because the manager is not in scope.</span></span>
2. <span data-ttu-id="6c8ed-119">In uno scenario **più domini AD**, il manager in Workday non è presente nello stesso dominio dell'utente.</span><span class="sxs-lookup"><span data-stu-id="6c8ed-119">In a **multiple AD domains** scenario, the manager in Workday is not present in the same domain as the user.</span></span>

<span data-ttu-id="6c8ed-120">Provare questa procedura per risolvere il problema:</span><span class="sxs-lookup"><span data-stu-id="6c8ed-120">Try these steps to resolve the issue:</span></span>

1. <span data-ttu-id="6c8ed-121">Se sono stati definiti filtri di ambito, verificare prima di tutto che il manager sia nell'ambito e che soddisfi la clausola di ambito.</span><span class="sxs-lookup"><span data-stu-id="6c8ed-121">If you have defined scoping filters, first check if the manager is in scope and that it satisfies the scoping clause.</span></span> <span data-ttu-id="6c8ed-122">Se il manager non soddisfa il filtro di ambito, modificare il filtro in modo che anche il responsabile sia nell'ambito dell'operazione di provisioning.</span><span class="sxs-lookup"><span data-stu-id="6c8ed-122">If the manager does not satisfy the scoping filter, change the filter so that the manager is also in scope of the provisioning operation.</span></span>
2. <span data-ttu-id="6c8ed-123">Se si hanno più domini Active Directory, il connettore presenta una limitazione nota di impossibilità a risolvere i riferimenti di manager tra domini.</span><span class="sxs-lookup"><span data-stu-id="6c8ed-123">If you have multiple AD domains, then the connector has a known limitation of inability to resolve cross-domain manager references.</span></span>

<span data-ttu-id="6c8ed-124">Per altri dettagli sulla configurazione di Workday per il provisioning automatizzato, vedere [Tutorial: configurare Workday per il provisioning utente automatico](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="6c8ed-124">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>













