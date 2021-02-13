---
title: Aggiungere Microsoft Edge a Microsoft Intune
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8240"
- "9004604"
ms.openlocfilehash: d56c65910d1c2170d3e0ce9676e913663701db96
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 02/10/2021
ms.locfileid: "50177999"
---
# <a name="add-microsoft-edge-to-microsoft-intune"></a><span data-ttu-id="57720-102">Aggiungere Microsoft Edge a Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="57720-102">Add Microsoft Edge to Microsoft Intune</span></span>

<span data-ttu-id="57720-103">Per distribuire, configurare, monitorare e proteggere Microsoft Edge per Windows 10, è necessario prima aggiungerlo a Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="57720-103">To be able to deploy, configure, monitor, and protect Microsoft Edge for Windows 10, you must first add it to Microsoft Intune.</span></span>

> [!IMPORTANT]
- <span data-ttu-id="57720-104">Intune supporta Microsoft Edge 77 e versioni successive.</span><span class="sxs-lookup"><span data-stu-id="57720-104">Intune supports Microsoft Edge 77 and later versions.</span></span>
- <span data-ttu-id="57720-105">Intune rileverà eventuali installazioni preesistenti di Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="57720-105">Intune will detect any pre-existing installations of Microsoft Edge.</span></span>
- <span data-ttu-id="57720-106">Se Microsoft Edge è installato nel contesto utente, un'installazione di sistema sovrascriverà l'installazione nel contesto utente.</span><span class="sxs-lookup"><span data-stu-id="57720-106">If Microsoft Edge is installed in user context, a system installation will overwrite the installation in user context.</span></span>
- <span data-ttu-id="57720-107">Se Microsoft Edge è installato nel contesto di sistema, verrà segnalato il completamento dell’installazione.</span><span class="sxs-lookup"><span data-stu-id="57720-107">If Microsoft Edge is installed in system context, the installation success will be reported.</span></span>
- <span data-ttu-id="57720-108">Per tutti i canali nel contesto utente, le versioni preinstallate di Microsoft Edge 77 e le versioni successive verranno sovrascritte da Microsoft Edge installato nel contesto di sistema.</span><span class="sxs-lookup"><span data-stu-id="57720-108">Pre-installed Microsoft Edge 77 and later versions, for all channels in user context, will be overwritten with Microsoft Edge installed in system context.</span></span>

<span data-ttu-id="57720-109">**Prerequisito**</span><span class="sxs-lookup"><span data-stu-id="57720-109">**Prerequisite**</span></span>

<span data-ttu-id="57720-110">Windows 10, versione 1709 o versioni successive</span><span class="sxs-lookup"><span data-stu-id="57720-110">Windows 10 version 1709 or later versions</span></span>

<span data-ttu-id="57720-111">**Procedura per aggiungere Microsoft Edge a Intune**</span><span class="sxs-lookup"><span data-stu-id="57720-111">**Steps to add Edge to Intune**</span></span>

1. <span data-ttu-id="57720-112">[Configurare l'app in Intune](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="57720-112">[Configure the app in Intune](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
2. <span data-ttu-id="57720-113">[Configurare le informazioni dell'app](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="57720-113">[Configure the app information](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
3. <span data-ttu-id="57720-114">[Configurare le impostazioni dell'app](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="57720-114">[Configure the app settings](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
4. <span data-ttu-id="57720-115">[Selezionare i tag dell’ambito (facoltativo)](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="57720-115">[Select the scope tags (optional)](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
5. <span data-ttu-id="57720-116">[Aggiungere l'app](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="57720-116">[Add the app](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>

<span data-ttu-id="57720-117">Per altre informazioni, vedere [Risoluzione dei problemi](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="57720-117">For more help, see [Troubleshooting](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>




