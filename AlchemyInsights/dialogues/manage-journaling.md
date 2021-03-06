---
title: Gestione dell'inserimento nel journal
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004299"
- "7677"
ms.openlocfilehash: 2fcd0f386d2da8cad19fcc9872482bb75fe00dd2
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/05/2021
ms.locfileid: "50509787"
---
# <a name="manage-journaling"></a><span data-ttu-id="eefc1-102">Gestione dell'inserimento nel journal</span><span class="sxs-lookup"><span data-stu-id="eefc1-102">Manage journaling</span></span>

<span data-ttu-id="eefc1-103">La creazione del journal consente alle organizzazioni di soddisfare i requisiti di conformità legale, normativa e organizzativa registrando le comunicazioni di posta elettronica in entrata e in uscita.</span><span class="sxs-lookup"><span data-stu-id="eefc1-103">Journaling can help your organization respond to legal, regulatory, and organizational compliance requirements by recording inbound and outbound email communications.</span></span> <span data-ttu-id="eefc1-104">Tenere presente che:</span><span class="sxs-lookup"><span data-stu-id="eefc1-104">Keep in mind:</span></span>

* <span data-ttu-id="eefc1-105">Per poter gestire [l'inserimento](https://go.microsoft.com/fwlink/?linkid=2115259) nel journal, è necessario disporre delle autorizzazioni Gestione organizzazione e Gestione record. [](https://go.microsoft.com/fwlink/?linkid=2115469)</span><span class="sxs-lookup"><span data-stu-id="eefc1-105">You need to have [Organization Management](https://go.microsoft.com/fwlink/?linkid=2115259) and [Records Management](https://go.microsoft.com/fwlink/?linkid=2115469) permissions before you can manage journaling.</span></span>
* <span data-ttu-id="eefc1-106">È necessario disporre di una cassetta del journal e, facoltativamente, di una cassetta del journaling alternativa configurata.</span><span class="sxs-lookup"><span data-stu-id="eefc1-106">You need to have a journal mailbox and (optionally) an alternate journaling mailbox configured.</span></span> <span data-ttu-id="eefc1-107">Per ulteriori informazioni, vedere [Configurare l'inserimento nel journal in Exchange Online.](https://go.microsoft.com/fwlink/?linkid=2115260)</span><span class="sxs-lookup"><span data-stu-id="eefc1-107">To learn more, see [Configure Journaling in Exchange Online](https://go.microsoft.com/fwlink/?linkid=2115260).</span></span>
* <span data-ttu-id="eefc1-108">In Exchange Online, esiste un limite al numero di regole del journal che è possibile creare.</span><span class="sxs-lookup"><span data-stu-id="eefc1-108">In Exchange Online, there's a limit to the number of journal rules that you can create.</span></span> <span data-ttu-id="eefc1-109">Per informazioni dettagliate, vedere Limiti delle regole del [journal, del trasporto e della posta in arrivo.](https://go.microsoft.com/fwlink/?linkid=2115261)</span><span class="sxs-lookup"><span data-stu-id="eefc1-109">For details, see [Journal, transport, and inbox rule limits](https://go.microsoft.com/fwlink/?linkid=2115261).</span></span>
* <span data-ttu-id="eefc1-p104">Exchange Online non supporta recapitando i rapporti del journal a una cassetta postale di Exchange Online. È necessario specificare l'indirizzo di posta elettronica di un locale archiviazione sistema o un servizio di archiviazione di terze parti come cassetta del journaling.</span><span class="sxs-lookup"><span data-stu-id="eefc1-p104">Exchange Online doesn't support delivering journal reports to an Exchange Online mailbox. You must specify the email address of an on-premises archiving system or a third-party archiving service as the journaling mailbox.</span></span>
