---
title: Uso dell'accesso condizionale con Intune
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6700002"
- "7680"
ms.openlocfilehash: 6e86c6b4c9c6adcbeac504acd5a10f2139d04237
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736769"
---
# <a name="using-conditional-access-with-intune"></a><span data-ttu-id="7c0f8-102">Uso dell'accesso condizionale con Intune</span><span class="sxs-lookup"><span data-stu-id="7c0f8-102">Using Conditional Access with Intune</span></span>

<span data-ttu-id="7c0f8-103">L'uso dell'accesso condizionale con Intune richiede 3 passaggi:</span><span class="sxs-lookup"><span data-stu-id="7c0f8-103">Using Conditional Access with Intune requires 3 steps:</span></span>

- [<span data-ttu-id="7c0f8-104">Crea criteri di conformità per definire le impostazioni che devono essere soddisfatte prima che il dispositivo venga considerato conforme. Ad esempio, un dispositivo deve avere un pin di almeno 6 cifre prima di essere considerato conforme.</span><span class="sxs-lookup"><span data-stu-id="7c0f8-104">Create a Compliance Policy to define settings that must be met before the device is considered compliant. For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [<span data-ttu-id="7c0f8-105">Creare criteri di accesso condizionale che definiscono quali risorse vengono protette e quali condizioni devono essere soddisfatte per accedere a tali risorse. Ad esempio, un dispositivo deve essere conforme prima di accedere alla posta elettronica aziendale.</span><span class="sxs-lookup"><span data-stu-id="7c0f8-105">Create a Conditional Access Policy that defines what resources are being protected, and what conditions need to be met to access those resources. For example, a device must be compliant before accessing corporate email.</span></span>](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [<span data-ttu-id="7c0f8-106">Verificare che i criteri di conformità e i criteri di accesso condizionale siano destinati ai gruppi di utenti desiderati. Potrebbe essere necessario creare gruppi specifici di utenti in Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="7c0f8-106">Ensure both Compliance Policies and Conditional Access Policies are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[<span data-ttu-id="7c0f8-107">Altre informazioni...</span><span class="sxs-lookup"><span data-stu-id="7c0f8-107">Read more...</span></span>](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
