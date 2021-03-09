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
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/08/2021
ms.locfileid: "50552357"
---
# <a name="submit-an-email-message-by-providing-the-network-message-id"></a><span data-ttu-id="67436-102">Inviare un messaggio di posta elettronica fornendo l'ID del messaggio di rete</span><span class="sxs-lookup"><span data-stu-id="67436-102">Submit an email message by providing the network message ID</span></span>

1. <span data-ttu-id="67436-103">Nel riquadro **a comparsa Nuovo invio** selezionare E-mail e ID messaggio di **rete.** </span><span class="sxs-lookup"><span data-stu-id="67436-103">In the **New submission** flyout, select **Email** and **Network Message ID**.</span></span>
2. <span data-ttu-id="67436-104">Seguire questa procedura per trovare l'ID messaggio per un messaggio di posta elettronica in Outlook:</span><span class="sxs-lookup"><span data-stu-id="67436-104">Follow these steps to find the message ID for an email message in Outlook:</span></span>
    1. <span data-ttu-id="67436-105">Fare doppio clic sul messaggio di posta elettronica per aprirlo.</span><span class="sxs-lookup"><span data-stu-id="67436-105">Double-click the email message to open it.</span></span>
    1. <span data-ttu-id="67436-106">Selezionare **Proprietà**  >  **file.**</span><span class="sxs-lookup"><span data-stu-id="67436-106">Select **File** > **Properties**.</span></span>
    1. <span data-ttu-id="67436-107">Aprire blocco note o un documento di Word vuoto e quindi copiare e incollare il contenuto trovato nella casella intestazioni **Internet** nel documento aperto per una maggiore visibilità.</span><span class="sxs-lookup"><span data-stu-id="67436-107">Open Notepad or a blank Word document, and then copy and paste the content found in the **Internet headers** box into the open document for better visibility.</span></span>
    1. <span data-ttu-id="67436-108">Individuare il **campo X-MS-Exchange-Organization-Network-Message-Id.**</span><span class="sxs-lookup"><span data-stu-id="67436-108">Locate the **X-MS-Exchange-Organization-Network-Message-Id** field.</span></span> <span data-ttu-id="67436-109">Il valore dopo **il parametro :** è l'ID necessario per l'invio.</span><span class="sxs-lookup"><span data-stu-id="67436-109">The value after the **:** is the ID you need for your submission.</span></span>
3. <span data-ttu-id="67436-110">In **Destinatari,** se il messaggio di posta elettronica è atterrato nella cartella posta indesiderata per tutti i destinatari di questo messaggio di posta elettronica, scegliere **Seleziona tutto.**</span><span class="sxs-lookup"><span data-stu-id="67436-110">Under **Recipients**, if the email landed in the junk mail folder for all recipients of this email, choose **Select All**.</span></span> <span data-ttu-id="67436-111">In caso contrario, selezionare solo l'utente che ha segnalato il problema.</span><span class="sxs-lookup"><span data-stu-id="67436-111">If not, select only the user who reported the issue.</span></span>
4. <span data-ttu-id="67436-112">In **Motivo dell'invio,** se si seleziona Deve essere **bloccato,** specificare se il messaggio deve essere stato bloccato come Posta **indesiderata,** **Phishing** o **Malware,** quindi selezionare **Invia.**</span><span class="sxs-lookup"><span data-stu-id="67436-112">Under **Reason for submission**, if you select **Should have been blocked**, specify whether the message should have been blocked as **Spam**, **Phishing**, or **Malware**, and then select **Submit**.</span></span>

<span data-ttu-id="67436-113">Per ulteriori informazioni, vedere Come inviare posta [indesiderata, phish, URL e file](https://go.microsoft.com/fwlink/?linkid=2101479)sospetti a Microsoft per l'analisi.</span><span class="sxs-lookup"><span data-stu-id="67436-113">To learn more, see [How to submit suspected spam, phish, URLs, and files to Microsoft for scanning](https://go.microsoft.com/fwlink/?linkid=2101479).</span></span>
