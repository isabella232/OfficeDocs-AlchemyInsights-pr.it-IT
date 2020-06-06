---
title: Problemi di accesso a Microsoft 365 Apps
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: 4e7612562d036f1c717817d3c883d6df80f86e2f
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579869"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="96cda-102">Risoluzione delle app Microsoft 365 "il modulo della piattaforma trusted del computer non funziona correttamente" messaggio</span><span class="sxs-lookup"><span data-stu-id="96cda-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="96cda-103">Per risolvere il problema, provare a eseguire le operazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="96cda-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="96cda-104">Installare gli aggiornamenti più recenti per [Windows](https://support.microsoft.com/help/4027667/windows-10-update) e [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="96cda-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="96cda-105">[Cancellare le credenziali di Office](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) utilizzando Gestione credenziali di Windows.</span><span class="sxs-lookup"><span data-stu-id="96cda-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="96cda-106">**Nota:** I percorsi del registro di sistema per Office 2016 sono stati modificati in 16,0.</span><span class="sxs-lookup"><span data-stu-id="96cda-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="96cda-107">(Es: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="96cda-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="96cda-108">Provare a eseguire il [processo di ripristino dell'utente](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) per correggere gli errori TPM (Trusted Platform Module).</span><span class="sxs-lookup"><span data-stu-id="96cda-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="96cda-109">Impostare EnableADAL = 0 eseguendo la procedura seguente:</span><span class="sxs-lookup"><span data-stu-id="96cda-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="96cda-110">Fare clic con il pulsante destro del mouse su Start, scegliere **Esegui**, digitare **Regedit**e quindi scegliere **OK**.</span><span class="sxs-lookup"><span data-stu-id="96cda-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="96cda-111">Selezionare **Sì** per consentire all'editor del registro di sistema di apportare modifiche al dispositivo.</span><span class="sxs-lookup"><span data-stu-id="96cda-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="96cda-112">Nell'editor del registro di sistema aggiungere un valore DWORD di **EnableADAL** con un'impostazione pari a **0** in HKEY_CURRENT_USER \software\microsoft\office\16.0\common\identity.</span><span class="sxs-lookup"><span data-stu-id="96cda-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="96cda-113">Per ulteriori informazioni, vedere [Connection issues in Sign-in after update to Office 2016 Build 16.0.7967 in Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="96cda-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>