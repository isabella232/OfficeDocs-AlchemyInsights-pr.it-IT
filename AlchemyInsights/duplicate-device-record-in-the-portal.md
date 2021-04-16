---
title: Record di dispositivo duplicati nel portale
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: e6f477807823e68965ce966faf0a6f50f9472f3d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814520"
---
# <a name="duplicate-device-record-in-the-portal"></a><span data-ttu-id="6782f-102">Record di dispositivo duplicati nel portale</span><span class="sxs-lookup"><span data-stu-id="6782f-102">Duplicate device record in the portal</span></span>

<span data-ttu-id="6782f-103">È possibile che nel portale siano presenti 2 record se il dispositivo non segnala correttamente lo stato della co-gestione al sito di Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="6782f-103">You may see 2 records for a device in the portal if the device does not correctly report the co-management status to the Configuration Manager site.</span></span> <span data-ttu-id="6782f-104">Per controllare lo stato della co-gestione di un dispositivo, esaminare la colonna **Con co-gestione** per il dispositivo nella console di Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="6782f-104">To check the co-management status of a device, review the **Co-managed** column for the device in the Configuration Manager console.</span></span> <span data-ttu-id="6782f-105">Se la colonna non è visibile, è possibile aggiungerla facendo clic con il pulsante destro del mouse su qualsiasi intestazione di colonna e selezionandola nell'elenco.</span><span class="sxs-lookup"><span data-stu-id="6782f-105">If the column is not visible, you may add it by right-clicking any of the column headers, and selecting it from the list.</span></span>

<span data-ttu-id="6782f-106">Il valore Con co-gestione **Sì**.</span><span class="sxs-lookup"><span data-stu-id="6782f-106">The Co-managed value must be **Yes**.</span></span> <span data-ttu-id="6782f-107">Se il valore è **No**, aprire l'applet del client di Configuration Manager nel dispositivo client e controllare la proprietà **Co-gestione** nella scheda Generale.</span><span class="sxs-lookup"><span data-stu-id="6782f-107">If the value is **No**, open the Configuration Manager client applet on the client device and check the **Co-management** property in the General tab.</span></span>

- <span data-ttu-id="6782f-108">Se il valore è **Abilitata**, i problemi sono associati alle comunicazioni del client nel punto di gestione.</span><span class="sxs-lookup"><span data-stu-id="6782f-108">If the value is **Enabled**, this indicates problems with client communication with the Management Point.</span></span> <span data-ttu-id="6782f-109">Esaminare il file **CcmMessaging.log** nel dispositivo per individuare i potenziali problemi di connettività.</span><span class="sxs-lookup"><span data-stu-id="6782f-109">Please review the **CcmMessaging.log** on the device to investigate potential connectivity issues.</span></span>

- <span data-ttu-id="6782f-110">Se il valore è **Disabilitata** e il dispositivo è registrato in Intune, assicurarsi che il dispositivo abbia ricevuto i criteri di co-gestione esaminando il file **CoManagementHandler.log** nel dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6782f-110">If the value is **Disabled** and the device is enrolled in Intune, please ensure that the device has received the Co-management policy by reviewing the **CoManagementHandler.log** on the device.</span></span>
