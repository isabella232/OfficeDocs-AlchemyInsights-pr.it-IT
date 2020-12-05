---
title: Operazioni da eseguire se le funzionalità di Azure non funzionano correttamente in Microsoft Edge
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004128"
- "7206"
ms.openlocfilehash: 463236bcd9ff480471604c992aa1ed1ed4ac2987
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/04/2020
ms.locfileid: "49576484"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a><span data-ttu-id="aef71-102">Operazioni da eseguire se le funzionalità di Azure non funzionano correttamente in Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="aef71-102">What to do if Azure features don't work properly in Microsoft Edge</span></span>

<span data-ttu-id="aef71-103">Microsoft Edge ha [problemi noti](https://go.microsoft.com/fwlink/?linkid=2140608) relativi alle aree di sicurezza e potrebbe influire sul modo in cui gli utenti di Azure accedono all'interfaccia di amministrazione di Windows.</span><span class="sxs-lookup"><span data-stu-id="aef71-103">Microsoft Edge has [known issues](https://go.microsoft.com/fwlink/?linkid=2140608) that are related to security zones and might affect how Azure users log in to Windows Admin Center.</span></span> <span data-ttu-id="aef71-104">Se si verificano problemi con le funzionalità di Azure con Microsoft Edge, provare a eseguire le operazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="aef71-104">If you're having trouble using Azure features with Microsoft Edge, try the following steps:</span></span>

1. <span data-ttu-id="aef71-105">Fare clic sul pulsante **Start** per cercare le **Opzioni Internet** e selezionarlo.</span><span class="sxs-lookup"><span data-stu-id="aef71-105">In the **Start** menu, search for **Internet Options** and select it.</span></span>
2. <span data-ttu-id="aef71-106">Nella finestra di dialogo **Proprietà Internet** passare alla scheda **sicurezza** .</span><span class="sxs-lookup"><span data-stu-id="aef71-106">In the **Internet Properties** dialog box, go to the **Security** tab.</span></span>
3. <span data-ttu-id="aef71-107">Selezionare l'area **siti attendibili** e quindi fare clic sul pulsante **siti** .</span><span class="sxs-lookup"><span data-stu-id="aef71-107">Select the **Trusted sites** zone and then select the **Sites** button.</span></span>
4. <span data-ttu-id="aef71-108">Nella finestra di dialogo **siti attendibili** aggiungere l'URL del gateway [https://login.microsoftonline.com](https://login.microsoftonline.com) e quindi fare [https://login.live.com](https://login.live.com) clic su **Chiudi**.</span><span class="sxs-lookup"><span data-stu-id="aef71-108">In the **Trusted sites** dialog box, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
5. <span data-ttu-id="aef71-109">Nella finestra di dialogo **Proprietà Internet** passare alla scheda **privacy** .</span><span class="sxs-lookup"><span data-stu-id="aef71-109">In the **Internet Properties** dialog box, go to the **Privacy** tab.</span></span>
6. <span data-ttu-id="aef71-110">Nella sezione **blocco popup** selezionare **Impostazioni**.</span><span class="sxs-lookup"><span data-stu-id="aef71-110">In the **Pop-up Blocker** section, select **Settings**.</span></span> <span data-ttu-id="aef71-111">Nella finestra di dialogo che si apre, aggiungere l'URL del gateway [https://login.microsoftonline.com](https://login.microsoftonline.com) e [https://login.live.com](https://login.live.com) quindi selezionare **Chiudi**.</span><span class="sxs-lookup"><span data-stu-id="aef71-111">In the dialog box that opens, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
