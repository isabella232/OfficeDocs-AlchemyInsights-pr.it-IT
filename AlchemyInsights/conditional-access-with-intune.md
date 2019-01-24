---
title: Accesso condizionale con Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 59f1aefaeec3d655b2388b00e7d58a8c2338504b
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/24/2019
ms.locfileid: "29476226"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="e09d3-102">Accesso condizionale con Intune</span><span class="sxs-lookup"><span data-stu-id="e09d3-102">Conditional Access with Intune</span></span>

<span data-ttu-id="e09d3-103">Utilizzo di **Access condizionale** con Intune richiede 3 passaggi:</span><span class="sxs-lookup"><span data-stu-id="e09d3-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="e09d3-p101">Creare un **Criterio di accesso condizionale** che definisce le risorse sono protetti e quali condizioni devono essere soddisfatti per accedere a tali risorse. Ad esempio, un dispositivo deve essere conforme prima di accedere alla posta elettronica aziendale.</span><span class="sxs-lookup"><span data-stu-id="e09d3-p101">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources. For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="e09d3-p102">Creare un **Criterio di conformità** per definire le impostazioni che devono essere soddisfatti prima che il dispositivo è considerato conforme. Ad esempio, un dispositivo deve disporre un pin di almeno 6 cifre prima che sia considerato compatibile.</span><span class="sxs-lookup"><span data-stu-id="e09d3-p102">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant. For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="e09d3-p103">Verificare i **Criteri di conformità** e **Criteri di accesso condizionale** destinate ai gruppi di utenti desiderati. Ciò può richiedere la creazione di gruppi di utenti specifici in Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e09d3-p103">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="e09d3-110">Altre informazioni</span><span class="sxs-lookup"><span data-stu-id="e09d3-110">Read more:</span></span>
  
- [<span data-ttu-id="e09d3-111">Procedure consigliate di accesso condizionale</span><span class="sxs-lookup"><span data-stu-id="e09d3-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="e09d3-112">Introduzione a Access condizionale</span><span class="sxs-lookup"><span data-stu-id="e09d3-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

