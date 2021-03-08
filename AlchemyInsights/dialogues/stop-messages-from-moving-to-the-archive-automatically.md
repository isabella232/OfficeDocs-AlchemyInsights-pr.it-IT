---
title: Impedire lo spostamento automatico dei messaggi nell'archivio
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
- "3100008"
- "7217"
ms.openlocfilehash: 2cb3e29dfd4f422e946b7887d4d44f373ff03794
ms.sourcegitcommit: 7fa9bf6f9fc7438791aa9241a440e5be817d4401
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/08/2021
ms.locfileid: "50522393"
---
# <a name="stop-messages-from-moving-to-the-archive-automatically"></a><span data-ttu-id="61027-102">Impedire lo spostamento automatico dei messaggi nell'archivio</span><span class="sxs-lookup"><span data-stu-id="61027-102">Stop messages from moving to the archive automatically</span></span>

<span data-ttu-id="61027-103">Se si utilizza un criterio di conservazione, è possibile modificare il periodo di validità della conservazione in tale criterio per impedire l'archiviazione automatica dei messaggi.</span><span class="sxs-lookup"><span data-stu-id="61027-103">If you are using a retention policy, you can change the retention age in that policy to stop messages from archiving automatically.</span></span> <span data-ttu-id="61027-104">Ecco come:</span><span class="sxs-lookup"><span data-stu-id="61027-104">Here's how:</span></span>

1. <span data-ttu-id="61027-105">[Nell'interfaccia di amministrazione di Exchange](https://go.microsoft.com/fwlink/?linkid=2059104)scegliere i tag di conservazione per la **gestione**  >  **della conformità.**</span><span class="sxs-lookup"><span data-stu-id="61027-105">In the [Exchange admin center](https://go.microsoft.com/fwlink/?linkid=2059104), choose **compliance management** > **retention tags**.</span></span> <span data-ttu-id="61027-106">Individuare il tag di conservazione Sposta nell'archivio.</span><span class="sxs-lookup"><span data-stu-id="61027-106">Locate your Move to Archive retention tag.</span></span>
2. <span data-ttu-id="61027-107">Nel tag di conservazione modificare il periodo di conservazione (periodo di archiviazione) in **Non** interrompere mai l'archiviazione automatica degli elementi da parte di un criterio di conservazione.</span><span class="sxs-lookup"><span data-stu-id="61027-107">In the retention tag, change the retention period (archive period) to **Never** to stop items from being automatically archived by a retention policy.</span></span>

> [!NOTE]
> <span data-ttu-id="61027-108">In questo modo verrà cambiata l'impostazione di archiviazione per tutte le cassette postali a cui è applicato questo tag di conservazione.</span><span class="sxs-lookup"><span data-stu-id="61027-108">This will change the archive setting for all mailboxes with this retention tag applied to them.</span></span>
