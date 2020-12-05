---
title: 'Ruoli RBAC '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "7265"
ms.openlocfilehash: 7c4c9d1a76f395dfb2f831d555199b76c354ca57
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/04/2020
ms.locfileid: "49576527"
---
# <a name="rbac-rules"></a><span data-ttu-id="af4c6-102">Regole RBAC</span><span class="sxs-lookup"><span data-stu-id="af4c6-102">RBAC rules</span></span>

<span data-ttu-id="af4c6-103">Se viene visualizzato l'errore di autorizzazione:</span><span class="sxs-lookup"><span data-stu-id="af4c6-103">If you get the permission error:</span></span> 

- <span data-ttu-id="af4c6-104">**Il client con ID oggetto non dispone dell'autorizzazione per eseguire l'azione su ambito (codice: AuthorizationFailed)**: quando si tenta di creare una risorsa, verificare di aver eseguito l'accesso con un utente a cui è assegnato un ruolo che disponga dell'autorizzazione di scrittura per la risorsa nell'ambito selezionato.</span><span class="sxs-lookup"><span data-stu-id="af4c6-104">**The client with object id does not have authorization to perform action over scope (code: AuthorizationFailed)**: when you try to create a resource, check that you are currently signed in with a user that is assigned a role that has write permission to the resource at the selected scope.</span></span> <span data-ttu-id="af4c6-105">Ad esempio, per gestire le macchine virtuali in un gruppo di risorse, è necessario avere il ruolo di [collaboratore della macchina virtuale](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) nel gruppo di risorse (o nell'ambito padre).</span><span class="sxs-lookup"><span data-stu-id="af4c6-105">For example, to manage virtual machines in a resource group, you should have the [Virtual Machine Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) role on the resource group (or parent scope).</span></span> <span data-ttu-id="af4c6-106">Per un elenco delle autorizzazioni per ogni ruolo incorporato, vedere [ruoli incorporati per le risorse di Azure](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="af4c6-106">For a list of the permissions for each built-in role, see [Built-in roles for Azure resources](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
- <span data-ttu-id="af4c6-107">**Non si dispone dell'autorizzazione necessaria per creare una richiesta di supporto**: quando si tenta di creare o aggiornare un ticket di supporto, verificare di aver eseguito l'accesso con un utente a cui è assegnato un ruolo che disponga dell'autorizzazione Microsoft. support/supportTickets/Write, ad esempio [supporto richieste collaboratore](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span><span class="sxs-lookup"><span data-stu-id="af4c6-107">**You don't have permission to create a support request**: when you try to create or update a support ticket, check that you are currently signed in with a user that is assigned a role that has the Microsoft.Support/supportTickets/write permission, such as [Support Request Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span></span>
- <span data-ttu-id="af4c6-108">**Non è possibile creare più assegnazioni di ruolo (codice: RoleAssignmentLimitExceeded)**: quando si tenta di assegnare un ruolo, provare a ridurre il numero di assegnazioni di ruolo assegnando invece i ruoli ai gruppi.</span><span class="sxs-lookup"><span data-stu-id="af4c6-108">**No more role assignments can be created (code: RoleAssignmentLimitExceeded)**: when you try to assign a role, try to reduce the number of role assignments by assigning roles to groups instead.</span></span> <span data-ttu-id="af4c6-109">Azure supporta fino a **2000** assegnazioni di ruolo per ogni sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="af4c6-109">Azure supports up to **2000** role assignments per subscription.</span></span>

<span data-ttu-id="af4c6-110">Per ulteriori informazioni sui ruoli RBAC di Azure, vedere [ruoli RBAC di Azure](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="af4c6-110">For more details on Azure RBAC roles, see [Azure RBAC roles](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
