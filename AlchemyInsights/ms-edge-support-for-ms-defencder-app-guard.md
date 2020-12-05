---
title: Supporto di Microsoft Edge per la protezione delle applicazioni Microsoft Defender
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/04/2020
ms.locfileid: "49576548"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a><span data-ttu-id="b5320-102">Supporto di Microsoft Edge per la protezione delle applicazioni Microsoft Defender</span><span class="sxs-lookup"><span data-stu-id="b5320-102">Microsoft Edge's support for Microsoft Defender Application Guard</span></span>

<span data-ttu-id="b5320-103">Progettata per Windows 10 e Microsoft Edge, Application Guard utilizza un approccio di isolamento hardware che consente a un utente di accedere a un sito non attendibile dall'interno di un contenitore isolato, Hyper-V abilitato, separato dal sistema operativo host.</span><span class="sxs-lookup"><span data-stu-id="b5320-103">Designed for Windows 10 and Microsoft Edge, Application Guard uses a hardware-isolation approach that lets a user navigate an untrusted site from inside an isolated, Hyper-V–enabled container, separated from the host operating system.</span></span>

<span data-ttu-id="b5320-104">Un amministratore dell'organizzazione definisce un elenco di siti attendibili, risorse cloud e reti interne.</span><span class="sxs-lookup"><span data-stu-id="b5320-104">An enterprise admin defines a list of trusted websites, cloud resources, and internal networks.</span></span> <span data-ttu-id="b5320-105">Quando un utente visita un sito non presente nell'elenco, Microsoft Edge aprirà il sito nel contenitore.</span><span class="sxs-lookup"><span data-stu-id="b5320-105">When a user visits a site that's not on the list, Microsoft Edge will open the site in the container.</span></span> <span data-ttu-id="b5320-106">Ciò significa che se il sito risulta essere dannoso, il PC host rimarrà protetto e l'utente malintenzionato non otterrà i dati dell'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="b5320-106">This means that if the site turns out to be malicious, the host PC will remain protected and the attacker won't get to the enterprise data.</span></span>

<span data-ttu-id="b5320-107">L'installazione delle estensioni nel contenitore è supportata da Microsoft Edge versione 81 e può essere controllata tramite un criterio.</span><span class="sxs-lookup"><span data-stu-id="b5320-107">Installation of extensions in the container is supported as of Microsoft Edge version 81, and it can be controlled via a policy.</span></span> <span data-ttu-id="b5320-108">L'indirizzo updateURL utilizzato nei criteri di ExtensionInstallForcelist deve essere aggiunto come risorsa neutra nei criteri di isolamento della rete utilizzati dalla protezione dell'applicazione.</span><span class="sxs-lookup"><span data-stu-id="b5320-108">The updateURL address that gets used in the ExtensionInstallForcelist policy should be added as a Neutral Resource in the Network Isolation policies used by Application Guard.</span></span>

<span data-ttu-id="b5320-109">Per altre informazioni, vedere [supporto Microsoft Edge per Microsoft Defender Application Guard](https://go.microsoft.com/fwlink/?linkid=2134229).</span><span class="sxs-lookup"><span data-stu-id="b5320-109">For more info, see [Microsoft Edge support for Microsoft Defender Application Guard](https://go.microsoft.com/fwlink/?linkid=2134229).</span></span>
