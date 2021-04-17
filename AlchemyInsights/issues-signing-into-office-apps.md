---
title: Problemi di accesso alle app di Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: c64cf2c9dbf63caad22e54ae801adc3ed8ff0f62
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833007"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="aebbf-102">Correzione delle app di Microsoft 365 "Il modulo Trusted Platform del computer non funziona correttamente"</span><span class="sxs-lookup"><span data-stu-id="aebbf-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="aebbf-103">Per risolvere il problema, provare a eseguire le operazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="aebbf-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="aebbf-104">Installare gli aggiornamenti più recenti per [Windows](https://support.microsoft.com/help/4027667/windows-10-update) e [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="aebbf-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="aebbf-105">[Cancellare le credenziali di Office](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) tramite Gestione credenziali di Windows.</span><span class="sxs-lookup"><span data-stu-id="aebbf-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="aebbf-106">**Nota:** I percorsi del Registro di sistema per Office 2016 sono stati modificati in 16.0.</span><span class="sxs-lookup"><span data-stu-id="aebbf-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="aebbf-107">(Ad esempio: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="aebbf-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="aebbf-108">Provare il [processo di ripristino degli](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) utenti per correggere gli errori TPM (Trusted Platform Module).</span><span class="sxs-lookup"><span data-stu-id="aebbf-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="aebbf-109">Impostare EnableADAL = 0 seguendo la procedura seguente:</span><span class="sxs-lookup"><span data-stu-id="aebbf-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="aebbf-110">Fai clic con il pulsante destro del mouse sul pulsante Start di Windows, scegli **Esegui,** digita **regedit** e quindi scegli **OK.**</span><span class="sxs-lookup"><span data-stu-id="aebbf-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="aebbf-111">Seleziona **Sì** per consentire all'editor del Registro di sistema di apportare modifiche al dispositivo.</span><span class="sxs-lookup"><span data-stu-id="aebbf-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="aebbf-112">Nell'editor del Registro di sistema aggiungi un valore DWORD **EnableADAL** con un'impostazione pari a **0** in HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="aebbf-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="aebbf-113">Per ulteriori informazioni, vedere [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)</span><span class="sxs-lookup"><span data-stu-id="aebbf-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>