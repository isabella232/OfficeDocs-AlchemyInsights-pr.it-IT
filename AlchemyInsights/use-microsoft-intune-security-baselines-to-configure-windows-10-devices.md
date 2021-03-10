---
title: Usare le baseline di sicurezza di Microsoft Intune per configurare i dispositivi Windows 10
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: b95454ec8ce8d0d69d1f55f7ce4adc596929e2de
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 03/10/2021
ms.locfileid: "50641621"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a><span data-ttu-id="ef5df-102">Usare le baseline di sicurezza di Microsoft Intune per configurare i dispositivi Windows 10</span><span class="sxs-lookup"><span data-stu-id="ef5df-102">Use the Microsoft Intune security baselines for configuring Windows 10 devices</span></span>

<span data-ttu-id="ef5df-103">Le baseline di sicurezza di Intune consentono di proteggere utenti e servizi</span><span class="sxs-lookup"><span data-stu-id="ef5df-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="ef5df-104">Le baseline di sicurezza sono gruppi di impostazioni preconfigurate di Windows usate per l'applicazione di un gruppo noto di impostazioni e valori predefiniti consigliati dai team di sicurezza pertinenti.</span><span class="sxs-lookup"><span data-stu-id="ef5df-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="ef5df-105">Creando un profilo della baseline di sicurezza in Intune, è possibile dare vita a un modello formato da più profili di configurazione dei dispositivi.</span><span class="sxs-lookup"><span data-stu-id="ef5df-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="ef5df-106">Quando vengono implementate baseline di sicurezza a gruppi di utenti o dispositivi, le impostazioni vengono applicate ai dispositivi con Windows 10 o versioni successive.</span><span class="sxs-lookup"><span data-stu-id="ef5df-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later versions.</span></span> <span data-ttu-id="ef5df-107">Ad esempio, le baseline di sicurezza della gestione dei dispositivi mobili di Microsoft (1) abilita automaticamente BitLocker per le unità rimovibili, (2) richiede la password per sbloccare un dispositivo e (3) disabilita l'autenticazione di base.</span><span class="sxs-lookup"><span data-stu-id="ef5df-107">For example, the Microsoft mobile device management (MDM) security baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="ef5df-108">Quando un valore predefinito non funziona per il proprio ambiente, è possibile personalizzare la baseline per applicare le impostazioni desiderate.</span><span class="sxs-lookup"><span data-stu-id="ef5df-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="ef5df-109">Le baseline di sicurezza consentono inoltre di stabilire un flusso di lavoro end-to-end in Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="ef5df-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="ef5df-110">Seguono alcuni vantaggi di questa funzionalità:</span><span class="sxs-lookup"><span data-stu-id="ef5df-110">The following are some benefits of this functionality:</span></span>
- <span data-ttu-id="ef5df-111">Una baseline di sicurezza include procedure ottimali e suggerimenti per le impostazioni che riguardano la sicurezza.</span><span class="sxs-lookup"><span data-stu-id="ef5df-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="ef5df-112">Dato che Intune lavora in partnership con il team di sicurezza di Windows che crea le baseline per i criteri di gruppo, questi suggerimenti si basano su linee guida solide e una comprovata esperienza.</span><span class="sxs-lookup"><span data-stu-id="ef5df-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="ef5df-113">Se non conosci bene Intune e non sai da dove cominciare, le baseline di sicurezza ti aiuteranno a creare e implementare rapidamente un profilo sicuro.</span><span class="sxs-lookup"><span data-stu-id="ef5df-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="ef5df-114">Se stai usando un criterio di gruppo, la migrazione a Intune per scopi correlati alla gestione è più semplice con le baseline di sicurezza, perché tali baseline di sicurezza sono predefinite in Intune e includono funzionalità per la gestione all'avanguardia.</span><span class="sxs-lookup"><span data-stu-id="ef5df-114">If you are currently using a group policy, then migrating to Intune for management purposes is much easier with security baselines, because these security baselines are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="ef5df-115">Per ulteriori informazioni, vedere [Baseline di sicurezza di Windows](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) e [Gestione dispositivi mobili](https://docs.microsoft.com/windows/client-management/mdm/).</span><span class="sxs-lookup"><span data-stu-id="ef5df-115">For more information, see [Windows security baselines](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](https://docs.microsoft.com/windows/client-management/mdm/).</span></span>