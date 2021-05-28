---
title: Prevenzione della perdita dei dati degli endpoint non distribuita sul dispositivo dell’utente
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11470"
- "9000292"
ms.openlocfilehash: 948835f5468b480536c176bfdf3b4eefb76b3bdb
ms.sourcegitcommit: c32233a1b7e6f1b07913d25f90189a58a8de2560
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 05/27/2021
ms.locfileid: "52694807"
---
# <a name="endpoint-dlp-not-deployed-to-users-device"></a><span data-ttu-id="4dd1a-102">Prevenzione della perdita dei dati degli endpoint non distribuita sul dispositivo dell’utente</span><span class="sxs-lookup"><span data-stu-id="4dd1a-102">Endpoint DLP not deployed to user's device</span></span>

<span data-ttu-id="4dd1a-103">Se l’impostazione della prevenzione della perdita di dati degli endpoint non è stata applicata sul dispositivo dell’utente, confermare che si soddisfano questi requisiti:</span><span class="sxs-lookup"><span data-stu-id="4dd1a-103">If the Endpoint data loss prevention (DLP) setting has not applied to a user's device, confirm you meet these requirements:</span></span>

- <span data-ttu-id="4dd1a-104">Windows 10 x64 build 1809 o installata successivamente sul dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4dd1a-104">Windows 10 x64 build 1809 or later is installed on the device.</span></span>
- <span data-ttu-id="4dd1a-105">Client antimalware versione 4.18.2009.7 o installata successivamente.</span><span class="sxs-lookup"><span data-stu-id="4dd1a-105">Anti-malware client version 4.18.2009.7 or later is installed.</span></span>
- <span data-ttu-id="4dd1a-106">Il dispositivo è **uno** dei seguenti:</span><span class="sxs-lookup"><span data-stu-id="4dd1a-106">The device is **one** of these:</span></span>
    
    - <span data-ttu-id="4dd1a-107">Aggiunto ad Azure Active Directory (Azure AD)</span><span class="sxs-lookup"><span data-stu-id="4dd1a-107">Azure Active Directory (Azure AD) joined</span></span>
    - <span data-ttu-id="4dd1a-108">Aggiunto ad Azure AD ibrido</span><span class="sxs-lookup"><span data-stu-id="4dd1a-108">Hybrid Azure AD joined</span></span>
    - <span data-ttu-id="4dd1a-109">Registrato ad Azure AD</span><span class="sxs-lookup"><span data-stu-id="4dd1a-109">AAD registered</span></span>

- <span data-ttu-id="4dd1a-110">Per applicare azioni dei criteri, assicurarsi che il browser Microsoft Edge Chromium sia installato sul dispositivo endpoint.</span><span class="sxs-lookup"><span data-stu-id="4dd1a-110">To enforce policy actions, make sure Microsoft Chromium Edge browser is installed on the endpoint device.</span></span>

<span data-ttu-id="4dd1a-111">Per requisiti aggiuntivi sulla prevenzione della perdita dei dati degli endpoint, passare a [Introduzione alla prevenzione della perdita di dati degli endpoint](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints).</span><span class="sxs-lookup"><span data-stu-id="4dd1a-111">For additional requirements for deploying Endpoint DLP, see [Get started with Endpoint data loss prevention](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints).</span></span>