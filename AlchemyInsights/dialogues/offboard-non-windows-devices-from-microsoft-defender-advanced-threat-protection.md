---
title: Offboard dei dispositivi non Windows da Microsoft Defender Advanced Threat Protection (ATP)
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 435957c555cd80155a985a49bd94b041a4ada31d
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/08/2021
ms.locfileid: "50530219"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a><span data-ttu-id="d788f-102">Offboard dei dispositivi non Windows da Microsoft Defender Advanced Threat Protection (ATP)</span><span class="sxs-lookup"><span data-stu-id="d788f-102">Offboard non-Windows devices from Microsoft Defender Advanced Threat Protection (ATP)</span></span>

<span data-ttu-id="d788f-103">Ecco come:</span><span class="sxs-lookup"><span data-stu-id="d788f-103">Here's how:</span></span>

1. <span data-ttu-id="d788f-104">Seguire la documentazione di terze parti per disconnettere la soluzione di terze parti da Microsoft Defender ATP.</span><span class="sxs-lookup"><span data-stu-id="d788f-104">Follow the third-party documentation for disconnecting the third-party solution from Microsoft Defender ATP.</span></span>
2. <span data-ttu-id="d788f-105">Dal tenant di Azure Active Directory, rimuovere le autorizzazioni per la soluzione di terze parti:</span><span class="sxs-lookup"><span data-stu-id="d788f-105">From your Azure Active Directory tenant, remove permissions for the third-party solution:</span></span>

    1. <span data-ttu-id="d788f-106">Accedere al [portale di Azure](https://go.microsoft.com/fwlink/?linkid=2125612).</span><span class="sxs-lookup"><span data-stu-id="d788f-106">Sign in to the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2125612).</span></span>
    1. <span data-ttu-id="d788f-107">Selezionare **Tutti i servizi** Azure Active  >  **Directory** Enterprise  >  **Applications.**</span><span class="sxs-lookup"><span data-stu-id="d788f-107">Select **All services** > **Azure Active Directory** > **Enterprise Applications**.</span></span>
    1. <span data-ttu-id="d788f-108">Seleziona l'applicazione che vuoi eseguire l'offboard.</span><span class="sxs-lookup"><span data-stu-id="d788f-108">Select the application you'd like to offboard.</span></span>
    1. <span data-ttu-id="d788f-109">Selezionare **Elimina**.</span><span class="sxs-lookup"><span data-stu-id="d788f-109">Select **Delete**.</span></span>

<span data-ttu-id="d788f-110">Per altre informazioni, vedi [Eseguire l'offboard dei dispositivi non Windows.](https://go.microsoft.com/fwlink/?linkid=2143630)</span><span class="sxs-lookup"><span data-stu-id="d788f-110">To learn more, see [Offboard non-Windows devices](https://go.microsoft.com/fwlink/?linkid=2143630).</span></span>
