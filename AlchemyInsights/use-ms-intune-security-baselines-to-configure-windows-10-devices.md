---
title: Utilizzare le linee di sicurezza di Microsoft Intune per configurare i dispositivi Windows 10
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: 24257f1ac5752df1598d08fcfdb95ee2642adfea
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/04/2020
ms.locfileid: "49571897"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="a4337-102">Utilizzare le linee di sicurezza di Microsoft Intune per configurare i dispositivi Windows 10</span><span class="sxs-lookup"><span data-stu-id="a4337-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="a4337-103">Le previsioni di sicurezza di Intune consentono di proteggere utenti e dispositivi.</span><span class="sxs-lookup"><span data-stu-id="a4337-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="a4337-104">Le linee di base per la sicurezza sono gruppi preconfigurati delle impostazioni di Windows utilizzati per applicare un gruppo conosciuto di impostazioni e valori predefiniti consigliati dai team di sicurezza rilevanti.</span><span class="sxs-lookup"><span data-stu-id="a4337-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="a4337-105">Creando un profilo di base di sicurezza in Intune, è possibile creare un modello costituito da più profili di configurazione dei dispositivi.</span><span class="sxs-lookup"><span data-stu-id="a4337-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="a4337-106">Quando si distribuiscono le linee di base di sicurezza ai gruppi di utenti o dispositivi, le impostazioni vengono applicate ai dispositivi eseguiti in Windows 10 o versioni successive.</span><span class="sxs-lookup"><span data-stu-id="a4337-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="a4337-107">Ad esempio, la linea di base di sicurezza MDM automaticamente (1) Abilita BitLocker per le unità rimovibili, (2) richiede la password per sbloccare un dispositivo e (3) disattiva l'autenticazione di base.</span><span class="sxs-lookup"><span data-stu-id="a4337-107">For example, MDM Security Baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="a4337-108">Quando un valore predefinito non funziona per l'ambiente in uso, personalizzare la linea di base per applicare le impostazioni necessarie.</span><span class="sxs-lookup"><span data-stu-id="a4337-108">When a default value doesn't work for your environment, customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="a4337-109">Le linee di base per la sicurezza consentono inoltre di stabilire un flusso di lavoro sicuro end-to-end in Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="a4337-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="a4337-110">Di seguito sono riportati alcuni vantaggi:</span><span class="sxs-lookup"><span data-stu-id="a4337-110">The following are some benefits of this:</span></span>

- <span data-ttu-id="a4337-111">Una previsione di sicurezza include le procedure consigliate e consigli per le impostazioni che influiscono sulla sicurezza.</span><span class="sxs-lookup"><span data-stu-id="a4337-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="a4337-112">Poiché Intune è partner del team di sicurezza di Windows che crea linee di base per i criteri di gruppo, questi suggerimenti si basano su una guida solida e un'esperienza estensiva.</span><span class="sxs-lookup"><span data-stu-id="a4337-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="a4337-113">Se si è nuovi di Intune e non si è sicuri di dove iniziare, quindi le linee di sicurezza di protezione consentiranno di creare e distribuire rapidamente un profilo sicuro.</span><span class="sxs-lookup"><span data-stu-id="a4337-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="a4337-114">Se attualmente si utilizza un criterio di gruppo, la migrazione a Intune per scopi di gestione è molto più semplice con le linee di base di sicurezza, perché sono integrate in Intune e comprendono funzionalità all'avanguardia per la gestione.</span><span class="sxs-lookup"><span data-stu-id="a4337-114">If you currently use a group policy, then migrating to Intune for management purposes is much easier with security baselines, because they are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="a4337-115">Per ulteriori informazioni, vedere [previsioni di sicurezza di Windows](https://go.microsoft.com/fwlink/?linkid=2141503) e [gestione dei dispositivi mobili](https://go.microsoft.com/fwlink/?linkid=2141701).</span><span class="sxs-lookup"><span data-stu-id="a4337-115">To learn more, see [Windows security baselines](https://go.microsoft.com/fwlink/?linkid=2141503) and [Mobile device management](https://go.microsoft.com/fwlink/?linkid=2141701).</span></span>