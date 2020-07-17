---
title: Informazioni sull'identità in Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: 2c4c2c836d18d2ab45e2368e778c793277b18aa0
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 07/16/2020
ms.locfileid: "45146774"
---
# <a name="about-identity-in-yammer"></a><span data-ttu-id="11fa1-102">Informazioni sull'identità in Yammer</span><span class="sxs-lookup"><span data-stu-id="11fa1-102">About identity in Yammer</span></span>

<span data-ttu-id="11fa1-103">È consigliabile eseguire la procedura seguente per evitare problemi correlati all'identità:</span><span class="sxs-lookup"><span data-stu-id="11fa1-103">It is recommended that all networks take the following steps to avoid identity-related issues:</span></span>

1. <span data-ttu-id="11fa1-104">Applicare l'identità di Office 365 dopo il provisioning degli account di Microsoft 365 per gli utenti in Azure AD per assicurarsi che tutti gli utenti accedano usando il proprio account di Microsoft 365 primario.</span><span class="sxs-lookup"><span data-stu-id="11fa1-104">Enforce Office 365 identity after provisioning Microsoft 365 accounts for users in Azure AD to ensure that all users sign in by using their primary Microsoft 365 account.</span></span> <span data-ttu-id="11fa1-105">Per alte informazioni, vedere [Applicare l'identità di Office 365 per gli utenti di Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span><span class="sxs-lookup"><span data-stu-id="11fa1-105">For more info, see [Enforce Office 365 identity for Yammer users](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span></span>
2. <span data-ttu-id="11fa1-106">Consolidare più reti di Yammer.</span><span class="sxs-lookup"><span data-stu-id="11fa1-106">Consolidate multiple Yammer networks.</span></span> <span data-ttu-id="11fa1-107">Le configurazioni legacy di Yammer consentono la connessione di più reti Yammer a un unico tenant.</span><span class="sxs-lookup"><span data-stu-id="11fa1-107">Legacy Yammer configurations permit multiple Yammer networks to be connected to one tenant.</span></span> <span data-ttu-id="11fa1-108">Per ulteriori informazioni, vedere [Migrazione di rete: consolidare più reti Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span><span class="sxs-lookup"><span data-stu-id="11fa1-108">For more info, see [Network migration - Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>
3. <span data-ttu-id="11fa1-109">È anche possibile applicare la licenza di Yammer per impedire agli utenti di Yammer che non dispongano di una licenza.</span><span class="sxs-lookup"><span data-stu-id="11fa1-109">Optionally, enforce licensing for Yammer to block users from Yammer if they don't have a license.</span></span> <span data-ttu-id="11fa1-110">Per ulteriori informazioni, vedere [Gestire le licenze utente di Yammer in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="11fa1-110">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span></span>
4. <span data-ttu-id="11fa1-111">Infine, controllare l'elenco degli utenti per le reti Yammer precedenti e sospendere gli utenti legacy.</span><span class="sxs-lookup"><span data-stu-id="11fa1-111">Finally, audit the user list for older Yammer networks and suspend legacy users.</span></span> <span data-ttu-id="11fa1-112">È consigliabile sospendere gli utenti, anziché eliminarli, perché l'eliminazione è irreversibile.</span><span class="sxs-lookup"><span data-stu-id="11fa1-112">It is recommended that you suspend (deactivate) users instead of deleting them, because deletion is irreversible.</span></span> <span data-ttu-id="11fa1-113">Per altre informazioni, vedere [Controllare gli utenti di Yammer nelle reti connesse a Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) e [Rimuovere gli utenti](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span><span class="sxs-lookup"><span data-stu-id="11fa1-113">For more info, see [Audit Yammer users in networks connected to Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) and [Remove users](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span></span>

<span data-ttu-id="11fa1-114">Configurando Yammer con questa procedura, è anche possibile configurare la rete Yammer per la modalità nativa di Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="11fa1-114">By configuring Yammer using these steps, you'll also be ready to configure your Yammer network for Native Mode for Microsoft 365.</span></span> <span data-ttu-id="11fa1-115">Per ulteriori informazioni, vedere [Configurare la rete Yammer per la modalità nativa di Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span><span class="sxs-lookup"><span data-stu-id="11fa1-115">For more info, see [Configure your Yammer network for Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span></span>