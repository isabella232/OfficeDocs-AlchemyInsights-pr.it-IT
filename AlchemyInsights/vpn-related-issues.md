---
title: Problemi correlati alla VPN
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
- "1545"
- "9000076"
ms.openlocfilehash: 134d78f30216dfd268c5999a5032b7d7ad1d7dd8
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 07/28/2020
ms.locfileid: "46505208"
---
# <a name="vpn-related-issues"></a><span data-ttu-id="c49a6-102">Problemi correlati alla VPN</span><span class="sxs-lookup"><span data-stu-id="c49a6-102">VPN related issues</span></span>

<span data-ttu-id="c49a6-103">L'implementazione efficace della connettività VPN per i client MDM dipende da un profilo distribuito che riflette correttamente i requisiti dell'infrastruttura VPN.</span><span class="sxs-lookup"><span data-stu-id="c49a6-103">Successful implementation of VPN connectivity for MDM clients depends on a deployed profile that correctly reflects the requirements of the VPN infrastructure.</span></span> <span data-ttu-id="c49a6-104">Per le impostazioni appropriate per le piattaforme client su cui si sta lavorando, vedere:</span><span class="sxs-lookup"><span data-stu-id="c49a6-104">For the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="c49a6-105">Impostazioni del dispositivo Windows 10 e Windows Holographic per aggiungere connessioni VPN usando Intune</span><span class="sxs-lookup"><span data-stu-id="c49a6-105">Windows 10 and Windows Holographic device settings to add VPN connections using Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[<span data-ttu-id="c49a6-106">Aggiungere impostazioni VPN sui dispositivi iOS e iPadOS in Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="c49a6-106">Add VPN settings on iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-ios)  
[<span data-ttu-id="c49a6-107">Impostazioni di dispositivi Android per configurare la VPN in Intune</span><span class="sxs-lookup"><span data-stu-id="c49a6-107">Android device settings to configure VPN in Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-android)  
[<span data-ttu-id="c49a6-108">Aggiungere impostazioni VPN sui dispositivi macOS in Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="c49a6-108">Add VPN settings on macOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

<span data-ttu-id="c49a6-109">Se il profilo VPN usa l'autenticazione basata su certificato, assicurarsi che il certificato radice e i profili dei certificati di autenticazione client collegati al profilo VPN vengano distribuiti correttamente.</span><span class="sxs-lookup"><span data-stu-id="c49a6-109">If your VPN profile uses certificate based authentication, make sure that the root certificate and client authentication certificate profiles linked to the VPN profile are deployed successfully.</span></span>

<span data-ttu-id="c49a6-110">**Problemi comuni**</span><span class="sxs-lookup"><span data-stu-id="c49a6-110">**Common Issues**</span></span>

<span data-ttu-id="c49a6-111">**Ho distribuito un profilo VPN in un dispositivo. Intune indica che l'operazione è riuscita, ma il dispositivo non è connesso alla rete VPN.**</span><span class="sxs-lookup"><span data-stu-id="c49a6-111">**I deployed a VPN profile to a device. Intune is showing that it was successful, but the device is not connecting to the VPN.**</span></span>

<span data-ttu-id="c49a6-112">Lo stato corretto indica che Intune ha distribuito correttamente il profilo come configurato.</span><span class="sxs-lookup"><span data-stu-id="c49a6-112">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="c49a6-113">Tuttavia, queste configurazioni potrebbero non corrispondere ai requisiti di rete e/o di autenticazione.</span><span class="sxs-lookup"><span data-stu-id="c49a6-113">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="c49a6-114">Rivedere i registri nel servizio di infrastruttura e autenticazione (sul server VPN e sul server NPS/RADIUS) per ulteriori dettagli sul tentativo di connessione.</span><span class="sxs-lookup"><span data-stu-id="c49a6-114">Review logs in the infrastructure and authentication service (on the VPN server and NPS/Radius server) for more details about the attempted connection.</span></span> <span data-ttu-id="c49a6-115">Potrebbe essere necessario usare il team dell'infrastruttura di rete o il fornitore di terze parti per raccogliere e rivedere i registri.</span><span class="sxs-lookup"><span data-stu-id="c49a6-115">You might need to work with your network infrastructure team, or the third-party VPN vendor, to gather and review logs.</span></span>

<span data-ttu-id="c49a6-116">**Quando configuro una VPN personalizzata per iOS, la funzionalità VPN per app non è disponibile.**</span><span class="sxs-lookup"><span data-stu-id="c49a6-116">**When I configure a custom VPN for iOS, the per-app VPN feature isn't made available.**</span></span>

<span data-ttu-id="c49a6-117">I dispositivi VPN per le app per dispositivi iOS di Intune sono attualmente disponibili per un elenco di provider e partner specifico, che deve inoltre soddisfare i prerequisiti dei certificati prima di poter configurare una VPN per app.</span><span class="sxs-lookup"><span data-stu-id="c49a6-117">Per-app VPN for iOS devices in Intune is currently available to a specific list of providers and partners, who must also meet the certificate prerequisites before configuring a per-app VPN.</span></span> <span data-ttu-id="c49a6-118">Per altre informazioni, vedere [Configurare una rete privata virtuale (VPN) per app per dispositivi iOS/iPadOS in Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span><span class="sxs-lookup"><span data-stu-id="c49a6-118">For more info, see [Set up per-app Virtual Private Network (VPN) for iOS/iPadOS devices in Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span></span> 

<span data-ttu-id="c49a6-119">Per altre informazioni su tutti i tipi di connessione VPN in Intune, vedere [Creare profili VPN per connettersi ai server VPN di Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="c49a6-119">For more info about all VPN connection types in Intune, see [Create VPN profiles to connect to VPN servers in Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span></span>  

<span data-ttu-id="c49a6-120">**La rete VPN iOS su richiesta non viene attivata quando si accede a un dominio configurato**</span><span class="sxs-lookup"><span data-stu-id="c49a6-120">**iOS On-Demand VPN is not triggering when a configured domain is accessed**</span></span>

<span data-ttu-id="c49a6-121">Per testare le impostazioni di VPN automatiche, impostare i seguenti valori:</span><span class="sxs-lookup"><span data-stu-id="c49a6-121">To test automatic VPN settings, set the following values:</span></span>

<span data-ttu-id="c49a6-122">Voglio eseguire queste operazioni: **Valutare ogni tentativo di connessione**</span><span class="sxs-lookup"><span data-stu-id="c49a6-122">I want to do the following: **Evaluate each connection attempt**</span></span> 

<span data-ttu-id="c49a6-123">Scegli se eseguire la connessione: **Eseguire la connessione se necessario**</span><span class="sxs-lookup"><span data-stu-id="c49a6-123">Choose whether to connect: **Connect if needed**</span></span>

<span data-ttu-id="c49a6-124">Quando gli utenti accedono a questi domini: **nome dominio** *di destinazione*</span><span class="sxs-lookup"><span data-stu-id="c49a6-124">When users access these domains: **target** *domain name*</span></span>

<span data-ttu-id="c49a6-125">Se la configurazione non riesce, aggiungere l'elemento seguente:</span><span class="sxs-lookup"><span data-stu-id="c49a6-125">If the above configuration is not successful, add the following element:</span></span>

<span data-ttu-id="c49a6-126">Quando l'URL non è raggiungibile, forzare la connessione VPN: **BADURL**</span><span class="sxs-lookup"><span data-stu-id="c49a6-126">When this URL is unreachable, force connect the VPN: **BADURL**</span></span>