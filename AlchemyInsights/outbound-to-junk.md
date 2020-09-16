---
title: Posta elettronica in uscita alla cartella posta indesiderata
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2697"
ms.assetid: ''
ms.openlocfilehash: 7e6f8d1a161d3eee398230750cc98a46579a56b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47769187"
---
# <a name="outbound-email-to-junk-email-folder"></a><span data-ttu-id="5e830-102">Posta elettronica in uscita alla cartella posta indesiderata</span><span class="sxs-lookup"><span data-stu-id="5e830-102">Outbound email to Junk Email folder</span></span>

<span data-ttu-id="5e830-103">Se i messaggi in uscita vengono contrassegnati come posta indesiderata, eseguire le operazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="5e830-103">If you're seeing outbound messages being marked as Junk, do the following steps:</span></span>

- <span data-ttu-id="5e830-104">Se non è stato già, è consigliabile [configurare le notifiche sui criteri di posta indesiderata in uscita](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy).</span><span class="sxs-lookup"><span data-stu-id="5e830-104">If you haven't already, consider [configuring outbound spam policy notifications](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy).</span></span>

- <span data-ttu-id="5e830-105">Utilizzare la [traccia dei messaggi](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) per verificare se il messaggio in uscita ha il valore di evento **posta indesiderata** con l'ulteriore dettaglio: **utilizza pool di recapito ad alto rischio**.</span><span class="sxs-lookup"><span data-stu-id="5e830-105">Use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) to see if the outbound message has the event value **Spam** with the additional detail: **Use high risk delivery pool**.</span></span>

  <span data-ttu-id="5e830-106">Per questi messaggi, controllare il contenuto del messaggio per vedere cosa può essere considerato come posta indesiderata.</span><span class="sxs-lookup"><span data-stu-id="5e830-106">For these messages, check the message content to see what might be considered spam.</span></span> <span data-ttu-id="5e830-107">Ad esempio, le firme possono talvolta causare problemi a molti utenti.</span><span class="sxs-lookup"><span data-stu-id="5e830-107">For example, signatures can sometimes cause problems for many users.</span></span>

  <span data-ttu-id="5e830-108">Se si dispone di più esempi di messaggi in uscita legittimi contrassegnati come posta indesiderata, aprire un ticket di supporto e chiedere all'agente di supporto di inviare i messaggi come falsi positivi ai nostri analisti di posta indesiderata.</span><span class="sxs-lookup"><span data-stu-id="5e830-108">If you have multiple examples of legitimate outbound messages that are being marked as Junk, open a support ticket and ask the support agent to submit your messages as false positives to our spam analysts.</span></span> <span data-ttu-id="5e830-109">Prepararsi a fornire messaggi di esempio che includano tutte le intestazioni dei messaggi.</span><span class="sxs-lookup"><span data-stu-id="5e830-109">Be prepared to provide sample messages that include all message headers.</span></span>
