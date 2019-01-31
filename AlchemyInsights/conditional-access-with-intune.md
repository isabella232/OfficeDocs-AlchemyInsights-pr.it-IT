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
ms.openlocfilehash: 3b50bc96a879017b62e42e1849f72e68408a0d9d
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/30/2019
ms.locfileid: "29662331"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="ef253-102">Accesso condizionale con Intune</span><span class="sxs-lookup"><span data-stu-id="ef253-102">Conditional Access with Intune</span></span>

<span data-ttu-id="ef253-103">Utilizzo di **Access condizionale** con Intune richiede 3 passaggi:</span><span class="sxs-lookup"><span data-stu-id="ef253-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="ef253-p101">Creare un **Criterio di accesso condizionale** che definisce le risorse sono protetti e quali condizioni devono essere soddisfatti per accedere a tali risorse. Ad esempio, un dispositivo deve essere conforme prima di accedere alla posta elettronica aziendale.</span><span class="sxs-lookup"><span data-stu-id="ef253-p101">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources. For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="ef253-p102">Creare un **Criterio di conformità** per definire le impostazioni che devono essere soddisfatti prima che il dispositivo è considerato conforme. Ad esempio, un dispositivo deve disporre un pin di almeno 6 cifre prima che sia considerato compatibile.</span><span class="sxs-lookup"><span data-stu-id="ef253-p102">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant. For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="ef253-p103">Verificare i **Criteri di conformità** e **Criteri di accesso condizionale** destinate ai gruppi di utenti desiderati. Ciò può richiedere la creazione di gruppi di utenti specifici in Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ef253-p103">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="ef253-110">Per ulteriori informazioni:</span><span class="sxs-lookup"><span data-stu-id="ef253-110">Read more:</span></span>
  
- [<span data-ttu-id="ef253-111">Procedure consigliate di accesso condizionale</span><span class="sxs-lookup"><span data-stu-id="ef253-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="ef253-112">Introduzione a Access condizionale</span><span class="sxs-lookup"><span data-stu-id="ef253-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

