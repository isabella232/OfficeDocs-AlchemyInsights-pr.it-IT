---
title: Inviare un messaggio di posta elettronica fornendo l'ID del messaggio di rete
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
ms.openlocfilehash: e4a0a3d9b4fede9198c8a235d05945b30a6e0807
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736476"
---
# <a name="submit-an-email-message-by-providing-the-network-message-id"></a><span data-ttu-id="7f9b5-102">Inviare un messaggio di posta elettronica fornendo l'ID del messaggio di rete</span><span class="sxs-lookup"><span data-stu-id="7f9b5-102">Submit an email message by providing the network message ID</span></span>

1. <span data-ttu-id="7f9b5-103">Nel riquadro **a comparsa Nuovo invio** selezionare E-mail e ID messaggio di **rete.** </span><span class="sxs-lookup"><span data-stu-id="7f9b5-103">In the **New submission** flyout, select **Email** and **Network Message ID**.</span></span>
2. <span data-ttu-id="7f9b5-104">Seguire questa procedura per trovare l'ID messaggio per un messaggio di posta elettronica in Outlook:</span><span class="sxs-lookup"><span data-stu-id="7f9b5-104">Follow these steps to find the message ID for an email message in Outlook:</span></span>
    1. <span data-ttu-id="7f9b5-105">Fare doppio clic sul messaggio di posta elettronica per aprirlo.</span><span class="sxs-lookup"><span data-stu-id="7f9b5-105">Double-click the email message to open it.</span></span>
    1. <span data-ttu-id="7f9b5-106">Selezionare **Proprietà**  >  **file**.</span><span class="sxs-lookup"><span data-stu-id="7f9b5-106">Select **File** > **Properties**.</span></span>
    1. <span data-ttu-id="7f9b5-107">Aprire blocco note o un documento vuoto di Word, quindi copiare e incollare il contenuto trovato nella casella Intestazioni **Internet** nel documento aperto per una migliore visibilità.</span><span class="sxs-lookup"><span data-stu-id="7f9b5-107">Open Notepad or a blank Word document, and then copy and paste the content found in the **Internet headers** box into the open document for better visibility.</span></span>
    1. <span data-ttu-id="7f9b5-108">Individuare il **campo X-MS-Exchange-Organization-Network-Message-Id.**</span><span class="sxs-lookup"><span data-stu-id="7f9b5-108">Locate the **X-MS-Exchange-Organization-Network-Message-Id** field.</span></span> <span data-ttu-id="7f9b5-109">Il valore dopo **: è** l'ID necessario per l'invio.</span><span class="sxs-lookup"><span data-stu-id="7f9b5-109">The value after the **:** is the ID you need for your submission.</span></span>
3. <span data-ttu-id="7f9b5-110">In **Destinatari**, se il messaggio di posta elettronica è atterrato nella cartella posta indesiderata per tutti i destinatari del messaggio di posta elettronica, scegliere **Seleziona tutto**.</span><span class="sxs-lookup"><span data-stu-id="7f9b5-110">Under **Recipients**, if the email landed in the junk mail folder for all recipients of this email, choose **Select All**.</span></span> <span data-ttu-id="7f9b5-111">In caso contrario, selezionare solo l'utente che ha segnalato il problema.</span><span class="sxs-lookup"><span data-stu-id="7f9b5-111">If not, select only the user who reported the issue.</span></span>
4. <span data-ttu-id="7f9b5-112">In **Motivo dell'invio,** se si seleziona Deve essere **bloccato,** specificare se il messaggio deve essere stato bloccato come **Posta** indesiderata, **Phishing** o **Malware** e quindi selezionare **Invia.**</span><span class="sxs-lookup"><span data-stu-id="7f9b5-112">Under **Reason for submission**, if you select **Should have been blocked**, specify whether the message should have been blocked as **Spam**, **Phishing**, or **Malware**, and then select **Submit**.</span></span>

<span data-ttu-id="7f9b5-113">Per ulteriori informazioni, vedere Come inviare a Microsoft la posta indesiderata sospetta, il phish, gli URL e [i file per l'analisi.](https://go.microsoft.com/fwlink/?linkid=2101479)</span><span class="sxs-lookup"><span data-stu-id="7f9b5-113">To learn more, see [How to submit suspected spam, phish, URLs, and files to Microsoft for scanning](https://go.microsoft.com/fwlink/?linkid=2101479).</span></span>
