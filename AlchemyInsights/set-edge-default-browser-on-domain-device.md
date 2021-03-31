---
title: Impostare Microsoft Edge come browser predefinito su un dispositivo aggiunto a un dominio
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: f51a455ea15b7bd92f548f2c1717be9888b43d07
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426838"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-domain-joined-device"></a><span data-ttu-id="a4f27-102">Impostare Microsoft Edge come browser predefinito su un dispositivo aggiunto a un dominio</span><span class="sxs-lookup"><span data-stu-id="a4f27-102">Set Microsoft Edge as the default browser on a domain-joined device</span></span>

<span data-ttu-id="a4f27-103">Impostare Microsoft Edge come browser predefinito:</span><span class="sxs-lookup"><span data-stu-id="a4f27-103">Set Microsoft Edge as the default browser:</span></span> 

1. <span data-ttu-id="a4f27-104">[Crea file di configurazione delle associazioni predefinite](https://go.microsoft.com/fwlink/?linkid=2132437) e archiviarlo localmente o in una condivisione di rete.</span><span class="sxs-lookup"><span data-stu-id="a4f27-104">[Create a default associations configuration file](https://go.microsoft.com/fwlink/?linkid=2132437) and store it locally or on a network share.</span></span>

1. <span data-ttu-id="a4f27-105">Aprire l'editor Criteri di gruppo e passare a **Configurazione computer** > **Modelli amministrativi** > **Componenti di Windows** > **Esplora file**.</span><span class="sxs-lookup"><span data-stu-id="a4f27-105">Open the Group Policy editor, and then go to **Computer Configuration** > **Administrative Templates** > **Windows Components** > **File Explorer**.</span></span>

1. <span data-ttu-id="a4f27-106">Selezionare **Imposta file di configurazione delle associazioni predefinite**.</span><span class="sxs-lookup"><span data-stu-id="a4f27-106">Select **Set a default associations configuration file**.</span></span>

1. <span data-ttu-id="a4f27-107">Selezionare **Impostazioni criterio**, quindi **Abilitato**.</span><span class="sxs-lookup"><span data-stu-id="a4f27-107">Select **Policy setting**, and then select **Enabled**.</span></span>

1. <span data-ttu-id="a4f27-108">In **Opzioni**, immettere la posizione del file di configurazione delle associazioni predefinite, quindi selezionare **OK**.</span><span class="sxs-lookup"><span data-stu-id="a4f27-108">Under **Options**, enter the location of your default associations configuration file, and then select **OK**.</span></span>
