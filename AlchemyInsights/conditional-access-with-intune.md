---
title: Accesso condizionale con Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: e147e7460ee6a786e577a43c0b8355fc27ee367b
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/15/2019
ms.locfileid: "36504998"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="c445b-102">Accesso condizionale con Intune</span><span class="sxs-lookup"><span data-stu-id="c445b-102">Conditional Access with Intune</span></span>

<span data-ttu-id="c445b-103">Se si utilizza **l'accesso condizionale** con Intune, è necessario eseguire tre passaggi:</span><span class="sxs-lookup"><span data-stu-id="c445b-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="c445b-104">Creare un **criterio di accesso condizionale** che definisce le risorse protette e quali condizioni devono essere soddisfatte per accedere a tali risorse.</span><span class="sxs-lookup"><span data-stu-id="c445b-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="c445b-105">Ad esempio, un dispositivo deve essere conforme prima di accedere alla posta elettronica aziendale.</span><span class="sxs-lookup"><span data-stu-id="c445b-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="c445b-106">Creare un **criterio di conformità** per definire le impostazioni che devono essere soddisfatte prima che il dispositivo venga considerato conforme.</span><span class="sxs-lookup"><span data-stu-id="c445b-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="c445b-107">Ad esempio, un dispositivo deve disporre di un pin di almeno 6 cifre prima di essere considerato conforme.</span><span class="sxs-lookup"><span data-stu-id="c445b-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="c445b-108">Garantire che i criteri di **conformità** e i **criteri di accesso condizionale** siano destinati ai gruppi di utenti desiderati.</span><span class="sxs-lookup"><span data-stu-id="c445b-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="c445b-109">Questo potrebbe richiedere la creazione di gruppi specifici di utenti in Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c445b-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="c445b-110">Per ulteriori informazioni, vedere:</span><span class="sxs-lookup"><span data-stu-id="c445b-110">Read more:</span></span>
  
- [<span data-ttu-id="c445b-111">Procedure consigliate per l'accesso condizionale</span><span class="sxs-lookup"><span data-stu-id="c445b-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="c445b-112">Guida introduttiva all'accesso condizionale</span><span class="sxs-lookup"><span data-stu-id="c445b-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

