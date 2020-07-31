---
title: Profili Wi-Fi di Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1548"
- "9000076"
ms.openlocfilehash: e5e1007abadb8ddb30ca110d465131ec791e44b7
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509073"
---
# <a name="intune-wi-fi-profiles"></a><span data-ttu-id="97241-102">Profili Wi-Fi di Intune</span><span class="sxs-lookup"><span data-stu-id="97241-102">Intune Wi-Fi profiles</span></span>

<span data-ttu-id="97241-103">L'implementazione efficace della connettività Wi-Fi per i client MDM dipende da un profilo distribuito correttamente che riflette i requisiti dell'infrastruttura Wi-Fi aziendale.</span><span class="sxs-lookup"><span data-stu-id="97241-103">Successful implementation of Wi-Fi connectivity for MDM clients depends on a correctly deployed profile that reflects the requirements of the corporate Wi-Fi infrastructure.</span></span> <span data-ttu-id="97241-104">Per verificare le impostazioni appropriate per le piattaforme client su cui si sta lavorando, si veda:</span><span class="sxs-lookup"><span data-stu-id="97241-104">To review the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="97241-105">Aggiungere impostazioni Wi-Fi per i dispositivi che utilizzano Android in Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="97241-105">Add Wi-Fi settings for devices running Android in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android)

[<span data-ttu-id="97241-106">Aggiungere impostazioni Wi-Fi per i dispositivi Android Enterprise dedicati e completamente gestiti in Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="97241-106">Add Wi-Fi settings for Android Enterprise dedicated and fully managed devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[<span data-ttu-id="97241-107">Aggiungere impostazioni Wi-Fi per i dispositivi iOS e iPadOS in Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="97241-107">Add Wi-Fi settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[<span data-ttu-id="97241-108">Aggiungere impostazioni Wi-Fi per dispositivi Windows 10 e successivi in Intune</span><span class="sxs-lookup"><span data-stu-id="97241-108">Add Wi-Fi settings for Windows 10 and later devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[<span data-ttu-id="97241-109">Aggiungere impostazioni Wi-Fi per dispositivi Windows in Intune</span><span class="sxs-lookup"><span data-stu-id="97241-109">Import Wi-Fi settings for Windows devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

<span data-ttu-id="97241-110">**Problemi comuni**</span><span class="sxs-lookup"><span data-stu-id="97241-110">**Common Issues**</span></span>

<span data-ttu-id="97241-111">**Si sta distribuendo un profilo Wi-Fi che dipende da un certificato distribuito specificato nel profilo Wi-Fi. Tuttavia, i profili di configurazione indicano uno stato di errore.**</span><span class="sxs-lookup"><span data-stu-id="97241-111">**I'm deploying a Wi-Fi profile that is dependent on a deployed certificate specified in the Wi-Fi profile. However, the configuration profiles are showing an error status.**</span></span>

<span data-ttu-id="97241-112">Controllare che il dispositivo abbia ricevuto il certificato.</span><span class="sxs-lookup"><span data-stu-id="97241-112">Check that your device received the certificate.</span></span>

1. <span data-ttu-id="97241-113">In Intune, andare su **Tutti i dispositivi** e selezionare il dispositivo > **Configurazione dispositivo**.</span><span class="sxs-lookup"><span data-stu-id="97241-113">In Intune, go to **All Devices** and select the device > **Device configuration**.</span></span>

2. <span data-ttu-id="97241-114">Controllare che tutti i profili previsti siano elencati e completati.</span><span class="sxs-lookup"><span data-stu-id="97241-114">Check that all expected profiles are listed and in a successful state.</span></span>

3. <span data-ttu-id="97241-115">Per un profilo Android, se nella catena di certificati sono presenti certificati intermedi, accertarsi che siano distribuiti ai dispositivi Android.</span><span class="sxs-lookup"><span data-stu-id="97241-115">For an Android profile, if you have intermediate certificates in your certificate chain, make sure they are deployed to Android devices.</span></span>

    <span data-ttu-id="97241-116">Per controllare lo stato del certificato, andare su **Configurazione dispositivo** > **Profili** > **Android CA intermedio** > **Proprietà** > **Certificato attendibile**.</span><span class="sxs-lookup"><span data-stu-id="97241-116">To check the certificate status, go to **Device configuration** > **Profiles** > **Android intermediate CA** > **Properties** > **Trusted Certificate**.</span></span>

<span data-ttu-id="97241-117">Se si continuano a visualizzare errori, rivedere le sezioni relative alle procedure e alla risoluzione dei problemi.</span><span class="sxs-lookup"><span data-stu-id="97241-117">If you continue to see errors, review the procedures and troubleshooting sections.</span></span> <span data-ttu-id="97241-118">Per maggiori informazioni, si veda [Panoramica per la risoluzione dei problemi relativi ai profili dei certificati SCEP con Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="97241-118">For more info, see [Overview for troubleshooting SCEP certificate profiles with Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span></span>

<span data-ttu-id="97241-119">**Si è distribuito un profilo Wi-Fi in un dispositivo. Intune indica che l'operazione è riuscita, ma il dispositivo non è connesso alla rete Wi-Fi.**</span><span class="sxs-lookup"><span data-stu-id="97241-119">**I deployed a Wi-Fi profile to a device. Intune is showing that it was successful, but the device is not connecting to the Wi-Fi.**</span></span>

<span data-ttu-id="97241-120">Lo stato corretto indica che Intune ha distribuito correttamente il profilo come configurato.</span><span class="sxs-lookup"><span data-stu-id="97241-120">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="97241-121">Tuttavia, queste configurazioni potrebbero non corrispondere ai requisiti di rete e/o di autenticazione.</span><span class="sxs-lookup"><span data-stu-id="97241-121">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="97241-122">Per maggiori dettagli sul tentativo di connessione, rivedere i registri nel servizio di infrastruttura e autenticazione (sul controller del punto di accesso al Wi-Fi e sul server NPS/Radius).</span><span class="sxs-lookup"><span data-stu-id="97241-122">For more details about the attempted connection, review logs in the infrastructure and authentication service (on the Wi-Fi Access point controller and NPS/Radius server).</span></span> <span data-ttu-id="97241-123">Potrebbe essere necessario collaborare con il team dell'infrastruttura di rete o il terzo fornitore del Wi-Fi per raccogliere e rivedere i registri.</span><span class="sxs-lookup"><span data-stu-id="97241-123">You might have to work with your network infrastructure team, or the third-party Wi-Fi vendor, to gather and review logs.</span></span>