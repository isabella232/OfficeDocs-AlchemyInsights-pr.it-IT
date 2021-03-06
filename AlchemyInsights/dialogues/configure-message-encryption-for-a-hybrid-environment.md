---
title: Configurare la crittografia dei messaggi per un ambiente ibrido
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 22c2468b7639680b447b6464431a79b69f7198c3
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/05/2021
ms.locfileid: "50510168"
---
# <a name="configure-message-encryption-for-a-hybrid-environment"></a><span data-ttu-id="37a83-102">Configurare la crittografia dei messaggi per un ambiente ibrido</span><span class="sxs-lookup"><span data-stu-id="37a83-102">Configure message encryption for a hybrid environment</span></span>

<span data-ttu-id="37a83-103">Per gli ambienti ibridi di Exchange, gli utenti locali possono inviare messaggi di posta elettronica crittografati utilizzando Office Message Encryption (OME) solo se la posta elettronica viene instradata tramite Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="37a83-103">For hybrid Exchange environments, on-premises users can send encrypted email using Office Message Encryption (OME) only if email is routed through Exchange Online.</span></span>

<span data-ttu-id="37a83-104">Per crittografare i messaggi di posta elettronica utilizzando OME, eseguire la procedura seguente:</span><span class="sxs-lookup"><span data-stu-id="37a83-104">To encrypt emails using OME, perform the following steps:</span></span>

1. <span data-ttu-id="37a83-105">Utilizzare la [procedura guidata di configurazione](https://docs.microsoft.com/Exchange/hybrid-configuration-wizard) ibrida per configurare l'ambiente ibrido.</span><span class="sxs-lookup"><span data-stu-id="37a83-105">Use the [Hybrid Configuration wizard](https://docs.microsoft.com/Exchange/hybrid-configuration-wizard) to set up your hybrid environment.</span></span> <span data-ttu-id="37a83-106">Non sono necessari passaggi speciali per la configurazione della crittografia.</span><span class="sxs-lookup"><span data-stu-id="37a83-106">No special steps are required for setting up encryption.</span></span>
2. <span data-ttu-id="37a83-107">[Configurare le regole del flusso di posta per la crittografia](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) come si farebbe normalmente.</span><span class="sxs-lookup"><span data-stu-id="37a83-107">[Set up your mail flow rules for encryption](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) like you normally would.</span></span>


