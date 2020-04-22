---
title: Accesso condizionale con Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: c9c47d71b2da3840504d5b28c7c9e067b4c05fa5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706025"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="03e28-102">Accesso condizionale con Intune</span><span class="sxs-lookup"><span data-stu-id="03e28-102">Conditional Access with Intune</span></span>

<span data-ttu-id="03e28-103">Se si utilizza **l'accesso condizionale** con Intune, è necessario eseguire tre passaggi:</span><span class="sxs-lookup"><span data-stu-id="03e28-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="03e28-104">Creare un **criterio di accesso condizionale** che definisce le risorse protette e quali condizioni devono essere soddisfatte per accedere a tali risorse.</span><span class="sxs-lookup"><span data-stu-id="03e28-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="03e28-105">Ad esempio, un dispositivo deve essere conforme prima di accedere alla posta elettronica aziendale.</span><span class="sxs-lookup"><span data-stu-id="03e28-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="03e28-106">Creare un **criterio di conformità** per definire le impostazioni che devono essere soddisfatte prima che il dispositivo venga considerato conforme.</span><span class="sxs-lookup"><span data-stu-id="03e28-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="03e28-107">Ad esempio, un dispositivo deve disporre di un pin di almeno 6 cifre prima di essere considerato conforme.</span><span class="sxs-lookup"><span data-stu-id="03e28-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="03e28-108">Garantire che i criteri di **conformità** e i **criteri di accesso condizionale** siano destinati ai gruppi di utenti desiderati.</span><span class="sxs-lookup"><span data-stu-id="03e28-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="03e28-109">Questo potrebbe richiedere la creazione di gruppi specifici di utenti in Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="03e28-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="03e28-110">Per ulteriori informazioni, vedere:</span><span class="sxs-lookup"><span data-stu-id="03e28-110">Read more:</span></span>
  
- [<span data-ttu-id="03e28-111">Procedure consigliate per l'accesso condizionale</span><span class="sxs-lookup"><span data-stu-id="03e28-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="03e28-112">Guida introduttiva all'accesso condizionale</span><span class="sxs-lookup"><span data-stu-id="03e28-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

