---
title: Accesso condizionale con Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 5eec5982118b4f0246afadf2af219b2d5f32f95c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47807663"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="6f449-102">Accesso condizionale con Intune</span><span class="sxs-lookup"><span data-stu-id="6f449-102">Conditional Access with Intune</span></span>

<span data-ttu-id="6f449-103">Se si utilizza  **l'accesso condizionale**  con Intune, è necessario eseguire tre passaggi:</span><span class="sxs-lookup"><span data-stu-id="6f449-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="6f449-104">Creare un  **criterio di conformità**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) per definire le impostazioni che devono essere soddisfatte prima che il dispositivo venga considerato conforme.</span><span class="sxs-lookup"><span data-stu-id="6f449-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="6f449-105">Ad esempio, un dispositivo deve disporre di un pin di almeno 6 cifre prima di essere considerato conforme.</span><span class="sxs-lookup"><span data-stu-id="6f449-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="6f449-106">Creare un **criterio di accesso condizionale**  che definisce le risorse protette e quali condizioni devono essere soddisfatte per accedere a tali risorse.</span><span class="sxs-lookup"><span data-stu-id="6f449-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="6f449-107">[Ad esempio,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  un dispositivo deve essere conforme prima di accedere alla posta elettronica aziendale.</span><span class="sxs-lookup"><span data-stu-id="6f449-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="6f449-108">Verificare che i criteri di **conformità**  e i  **criteri di accesso condizionale**  siano destinati ai gruppi di utenti desiderati.</span><span class="sxs-lookup"><span data-stu-id="6f449-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="6f449-109">Questo potrebbe richiedere la creazione di gruppi specifici di utenti in Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="6f449-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="6f449-110">**Collegamenti utili:**</span><span class="sxs-lookup"><span data-stu-id="6f449-110">**Helpful links:**</span></span>

[<span data-ttu-id="6f449-111">Panoramica della conformità del dispositivo</span><span class="sxs-lookup"><span data-stu-id="6f449-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="6f449-112">Risoluzione dei problemi relativi all'autorità di certificazione</span><span class="sxs-lookup"><span data-stu-id="6f449-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="6f449-113">Risoluzione dei problemi relativi ai criteri</span><span class="sxs-lookup"><span data-stu-id="6f449-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="6f449-114">Per proteggere la posta elettronica (Exchange Online) dall'accesso da dispositivi non conformi, è necessario seguire entrambi i documenti:</span><span class="sxs-lookup"><span data-stu-id="6f449-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="6f449-115">Protezione dell'accesso alla posta elettronica dai dispositivi tramite EAS</span><span class="sxs-lookup"><span data-stu-id="6f449-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="6f449-116">Protezione dell'accesso tramite posta elettronica da dispositivi che utilizzano client di autenticazione moderni come Outlook</span><span class="sxs-lookup"><span data-stu-id="6f449-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)