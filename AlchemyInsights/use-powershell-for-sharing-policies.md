---
title: Usare PowerShell per i criteri di condivisione di criteri e relazioni dell'organizzazione
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
- "3800014"
- "898"
ms.openlocfilehash: 378dedb332ced2c86899401c54726eb6b7e25d08
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47773419"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a><span data-ttu-id="c96a9-102">Usare PowerShell per i criteri di condivisione di criteri e relazioni dell'organizzazione</span><span class="sxs-lookup"><span data-stu-id="c96a9-102">Use PowerShell for Sharing policies and Organization relationships</span></span>


<span data-ttu-id="c96a9-103">Per le relazioni organizzative, consultare la sintassi dettagliata e le informazioni sui parametri per: [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship) e [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span><span class="sxs-lookup"><span data-stu-id="c96a9-103">For Organization relationships please review the detailed syntax and parameter information for : [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  AND  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span></span>

<span data-ttu-id="c96a9-104">Per creare criteri di condivisione usare [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span><span class="sxs-lookup"><span data-stu-id="c96a9-104">To create sharing policy use [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span></span> <span data-ttu-id="c96a9-105">Per [applicare un criterio di condivisione a una cassetta postale o a un utente](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes) è necessario usare una combinazione di [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) e [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) con il criterio appena creato.</span><span class="sxs-lookup"><span data-stu-id="c96a9-105">To  [apply a sharing policy to a mailbox or user](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  you need to use a combination of  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) and [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) with the newly created policy.</span></span> <span data-ttu-id="c96a9-106">Per [modificare, disabilitare o rimuovere un criterio di condivisione](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy) è necessario usare [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) e [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span><span class="sxs-lookup"><span data-stu-id="c96a9-106">To  [modify, disable or remove a sharing policy](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  you need to use  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) and [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span></span>

<span data-ttu-id="c96a9-107">**Per informazioni complete su questo argomento, vedere:**</span><span class="sxs-lookup"><span data-stu-id="c96a9-107">**For full understanding of this topic please read:**</span></span>

[<span data-ttu-id="c96a9-108">Condivisione in Exchange Online</span><span class="sxs-lookup"><span data-stu-id="c96a9-108">Sharing in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing)