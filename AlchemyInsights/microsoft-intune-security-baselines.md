---
title: Usare Microsoft Intune di sicurezza per configurare Windows 10 dispositivi
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: 88525fccd6dcde0cb3949e348d1f2a7df3ee7ce7
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/06/2021
ms.locfileid: "52783230"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="2d72b-102">Usare Microsoft Intune di sicurezza per configurare Windows 10 dispositivi</span><span class="sxs-lookup"><span data-stu-id="2d72b-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="2d72b-103">Le baseline di sicurezza di Intune consentono di proteggere utenti e servizi</span><span class="sxs-lookup"><span data-stu-id="2d72b-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="2d72b-104">Le linee di base della sicurezza sono gruppi preconfigurato delle impostazioni di Windows utilizzati per applicare un gruppo noto di impostazioni e valori predefiniti consigliati dai team di sicurezza pertinenti.</span><span class="sxs-lookup"><span data-stu-id="2d72b-104">Security baselines are Windows settings pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="2d72b-105">Creando un profilo della baseline di sicurezza in Intune, è possibile dare vita a un modello formato da più profili di configurazione dei dispositivi.</span><span class="sxs-lookup"><span data-stu-id="2d72b-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="2d72b-106">Quando distribuisci linee di base per la sicurezza a gruppi di utenti o dispositivi, le impostazioni vengono applicate ai dispositivi eseguiti in Windows 10 o versioni successive.</span><span class="sxs-lookup"><span data-stu-id="2d72b-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="2d72b-107">Ad esempio, la linea di base di sicurezza microsoft per la gestione dei dispositivi mobili (MDM) abilita automaticamente il BitLocker per le unità rimovibili, richiede la password per sbloccare un dispositivo e disabilita l'autenticazione di base.</span><span class="sxs-lookup"><span data-stu-id="2d72b-107">For example, the Microsoft mobile device management (MDM) security baseline automatically enables BitLocker for removable drives, requires the password for unlocking a device, and disables basic authentication.</span></span> <span data-ttu-id="2d72b-108">Quando un valore predefinito non funziona per il proprio ambiente, è possibile personalizzare la baseline per applicare le impostazioni desiderate.</span><span class="sxs-lookup"><span data-stu-id="2d72b-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="2d72b-109">Le baseline di sicurezza consentono inoltre di stabilire un flusso di lavoro end-to-end in Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="2d72b-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="2d72b-110">Una baseline di sicurezza include procedure ottimali e suggerimenti per le impostazioni che riguardano la sicurezza.</span><span class="sxs-lookup"><span data-stu-id="2d72b-110">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="2d72b-111">Intune collabora con il team di sicurezza di Windows che crea linee di base per i criteri di gruppo, quindi questi suggerimenti si basano su solide indicazioni ed esperienze approfondite.</span><span class="sxs-lookup"><span data-stu-id="2d72b-111">Intune partners with the Windows security team that creates baselines for group policies, so these recommendations are based on solid guidance and extensive experience.</span></span>

<span data-ttu-id="2d72b-112">Se non si ha una nuova versione di Intune e non si è certi di dove iniziare, le linee di base della sicurezza consentono di creare e distribuire rapidamente un profilo sicuro.</span><span class="sxs-lookup"><span data-stu-id="2d72b-112">If you're new to Intune and unsure of where to start, security baselines help you quickly create and deploy a secure profile.</span></span> <span data-ttu-id="2d72b-113">Se attualmente si usano criteri di gruppo, la migrazione a Intune per scopi di gestione è molto più semplice con le linee di base della sicurezza perché sono integrate in Intune e includono funzionalità di gestione all'avanguardia.</span><span class="sxs-lookup"><span data-stu-id="2d72b-113">If you currently use a group policy, migrating to Intune for management purposes is much easier with security baselines because they are built into Intune and include cutting-edge management capabilities.</span></span>

<span data-ttu-id="2d72b-114">Per altre informazioni, vedi Linee [di base per la sicurezza di Windows](/windows/security/threat-protection/windows-security-baselines) e Gestione dei dispositivi [mobili.](/windows/client-management/mdm/)</span><span class="sxs-lookup"><span data-stu-id="2d72b-114">To learn more, see [Windows security baselines](/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](/windows/client-management/mdm/).</span></span>

