---
title: Ripristinare il file PST prima di importarlo
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
- "1226"
- "1800027"
ms.assetid: ''
ms.openlocfilehash: 1ed37192a6b054b745fd48fbc01a6b00fa7074ed
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799100"
---
# <a name="repair-pst-file-before-importing"></a><span data-ttu-id="94e85-102">Ripristinare il file PST prima di importarlo</span><span class="sxs-lookup"><span data-stu-id="94e85-102">Repair .pst file before importing</span></span>

<span data-ttu-id="94e85-103">Prima di importare un file. pst in Outlook, verificare che il file non sia danneggiato ripristinando il file:</span><span class="sxs-lookup"><span data-stu-id="94e85-103">Before you import a .pst file in Outlook, verify the file is not corrupted by repairing the file:</span></span>

1. <span data-ttu-id="94e85-104">Chiudere Outlook.</span><span class="sxs-lookup"><span data-stu-id="94e85-104">Exit Outlook.</span></span>

2. <span data-ttu-id="94e85-105">Individuare ed eseguire `Scanpst.exe` la cartella del programma di Office (C:\Program Files (x86) \Microsoft Office\root\Office \<Version\> o c:\Programmi\Microsoft Office\root\Office \<Version\> ).</span><span class="sxs-lookup"><span data-stu-id="94e85-105">Find and run `Scanpst.exe` in your Office program folder (C:\Program Files (x86)\Microsoft Office\root\Office\<Version\> or C:\Program Files\Microsoft Office\root\Office\<Version\>).</span></span>

3. <span data-ttu-id="94e85-106">Nello **strumento di ripristino Posta in arrivo di Microsoft Outlook**fare clic su **Sfoglia** per individuare il file. pst (ad esempio, in C:\Users \\<nomeutente \> \AppData\Local\Microsoft\Outlook).</span><span class="sxs-lookup"><span data-stu-id="94e85-106">In the **Microsoft Outlook Inbox Repair tool**, click **Browse** to find the .pst file (for example, in C:\Users\\<username\>\AppData\Local\Microsoft\Outlook).</span></span> <span data-ttu-id="94e85-107">Selezionare il file con estensione pst e quindi fare clic su **Apri**.</span><span class="sxs-lookup"><span data-stu-id="94e85-107">Select the .pst file and then click **Open**.</span></span>

4. <span data-ttu-id="94e85-108">Fare clic su **Avvia** per avviare l'analisi.</span><span class="sxs-lookup"><span data-stu-id="94e85-108">Click **Start** to begin the scan.</span></span>

5. <span data-ttu-id="94e85-109">Se si verificano errori nel file, fare clic su **Ripristina**e quindi fare clic su **OK** al termine del ripristino.</span><span class="sxs-lookup"><span data-stu-id="94e85-109">If errors are found in the file, click **Repair**, and then click **OK** when the repair is complete.</span></span>

6. <span data-ttu-id="94e85-110">Provare a importare di nuovo il file. pst in Outlook.</span><span class="sxs-lookup"><span data-stu-id="94e85-110">Try to import the .pst file in Outlook again.</span></span>

<span data-ttu-id="94e85-111">Per ulteriori informazioni, vedere [ripristinare i file di dati di Outlook](https://support.office.com/article/25663bc3-11ec-4412-86c4-60458afc5253) e [correggere i problemi relativi all'importazione di un file PST di Outlook](https://support.office.com/article/2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span><span class="sxs-lookup"><span data-stu-id="94e85-111">For more information, see [Repair Outlook data files](https://support.office.com/article/25663bc3-11ec-4412-86c4-60458afc5253) and [Fix problems importing an Outlook .pst file](https://support.office.com/article/2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span></span>
