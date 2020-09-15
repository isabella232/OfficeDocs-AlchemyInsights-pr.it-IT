---
title: Utilizzo dei profili di posta elettronica con Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 92d91de5d369eb9d0ffde2580b75376035a6945b
ms.sourcegitcommit: 483444ab35ab0e4d410d121562045efde47aa61a
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47653292"
---
# <a name="using-email-profiles-with-intune"></a><span data-ttu-id="32fa5-102">Utilizzo dei profili di posta elettronica con Intune</span><span class="sxs-lookup"><span data-stu-id="32fa5-102">Using email profiles with Intune</span></span>

<span data-ttu-id="32fa5-103">Intune può essere usato per creare e distribuire profili di posta elettronica per il client di posta elettronica nativo (predefinito) su più piattaforme di dispositivi.</span><span class="sxs-lookup"><span data-stu-id="32fa5-103">Intune can be used to create and deploy email profiles for the native (built-in) email client on multiple device platforms.</span></span>

<span data-ttu-id="32fa5-104">Per informazioni su alcune delle restrizioni associate ai profili di posta elettronica, incluse informazioni su come è gestita la presenza dei profili esistenti e come rimuovere i profili di posta elettronica, si veda [Aggiungere le impostazioni di posta elettronica ai dispositivi con Intune](https://docs.microsoft.com/intune/email-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="32fa5-104">For info about some of the restrictions associated with email profiles, including how the presence of existing profiles are handled and how to remove email profiles, see [Add email settings to devices using Intune](https://docs.microsoft.com/intune/email-settings-configure).</span></span>

<span data-ttu-id="32fa5-105">Per altre informazioni su come creare profili di posta elettronica per ogni piattaforma del dispositivo, si veda:</span><span class="sxs-lookup"><span data-stu-id="32fa5-105">For more info about how to create email profiles for each device platform, see:</span></span>

[<span data-ttu-id="32fa5-106">Impostazioni dei dispositivi Android per configurare la posta elettronica, l'autenticazione e la sincronizzazione in Intune</span><span class="sxs-lookup"><span data-stu-id="32fa5-106">Android device settings to configure email, authentication, and synchronization in Intune</span></span>](https://docs.microsoft.com/intune/email-settings-android)  
[<span data-ttu-id="32fa5-107">Aggiungere impostazioni di posta elettronica per i dispositivi iOS e iPadOS in Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="32fa5-107">Add e-mail settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-ios)  
[<span data-ttu-id="32fa5-108">Impostazioni del profilo di posta elettronica in Microsoft Intune per dispositivi che utilizzano Windows Phone 8.1</span><span class="sxs-lookup"><span data-stu-id="32fa5-108">Email profile settings in Microsoft Intune for devices running Windows Phone 8.1</span></span>](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[<span data-ttu-id="32fa5-109">Impostazioni del profilo di posta elettronica per i dispositivi che utilizzano Windows 10 in Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="32fa5-109">Email profile settings for devices running Windows 10 in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-windows-10)

<span data-ttu-id="32fa5-110">**Problema di sincronizzazione comune**</span><span class="sxs-lookup"><span data-stu-id="32fa5-110">**Common syncing issue**</span></span>

<span data-ttu-id="32fa5-111">**Il profilo di posta elettronica Knox su Android impedisce che i contatti, il calendario e le attività degli utenti siano sincronizzati con i dispositivi degli utenti.**</span><span class="sxs-lookup"><span data-stu-id="32fa5-111">**A KNOX on Android email profile prevents user Contacts, Calendar, and Tasks, from being sync'd to user devices.**</span></span>

<span data-ttu-id="32fa5-112">Il profilo di posta elettronica Knox su Android offre agli amministratori la possibilità di decidere quali tipi di contenuto vengano sincronizzati con il dispositivo, configurando ogni tipo di contenuto in modo che sia abilitato.</span><span class="sxs-lookup"><span data-stu-id="32fa5-112">The KNOX on Android KNOX email profile offers the admin the option to decide which content types are sync'd to the device by setting each to enabled.</span></span>

<span data-ttu-id="32fa5-113">Se l'impostazione di uno dei tipi di contenuto è impostata su **Non configurato** (impostazione predefinita), quel tipo di contenuto non viene sincronizzato automaticamente.</span><span class="sxs-lookup"><span data-stu-id="32fa5-113">If the setting for any of the content types is set to **Not configured** (the default), that content type is not sync'd automatically.</span></span> <span data-ttu-id="32fa5-114">Un utente può abilitare manualmente il tipo di contenuto che vuole sincronizzare direttamente nel dispositivo, ma tale configurazione viene sovrascritta dall'impostazione dei criteri di Intune e la sincronizzazione si interrompe per quel tipo di contenuto.</span><span class="sxs-lookup"><span data-stu-id="32fa5-114">A user might enable the content type they want directly on the device manually, but that configuration is overwritten by the Intune policy setting, and the sync stops for that content type.</span></span>

