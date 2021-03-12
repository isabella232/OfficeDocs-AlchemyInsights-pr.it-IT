---
title: Problemi di accesso alle app di Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: d736c6c687695824f0ab37b8ffdc8456065353b0
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709110"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="82a18-102">Correzione del messaggio "Il modulo piattaforma attendibile del computer non funziona correttamente" delle app di Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="82a18-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="82a18-103">Per risolvere il problema, provare a eseguire le operazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="82a18-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="82a18-104">Installare gli aggiornamenti più recenti per [Windows](https://support.microsoft.com/help/4027667/windows-10-update) e [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)</span><span class="sxs-lookup"><span data-stu-id="82a18-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="82a18-105">[Cancellare le credenziali di Office](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) tramite Gestione credenziali di Windows.</span><span class="sxs-lookup"><span data-stu-id="82a18-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="82a18-106">**Nota:** I percorsi del Registro di sistema per Office 2016 sono stati modificati in 16.0.</span><span class="sxs-lookup"><span data-stu-id="82a18-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="82a18-107">(Ad esempio: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="82a18-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="82a18-108">Provare il [processo di ripristino degli](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) utenti per correggere gli errori di Trusted Platform Module (TPM).</span><span class="sxs-lookup"><span data-stu-id="82a18-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="82a18-109">Impostare EnableADAL = 0 seguendo la procedura seguente:</span><span class="sxs-lookup"><span data-stu-id="82a18-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="82a18-110">Fare clic con il pulsante destro del mouse sul pulsante Start di Windows, scegliere **Esegui,** digitare **regedit** e quindi scegliere **OK.**</span><span class="sxs-lookup"><span data-stu-id="82a18-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="82a18-111">Seleziona **Sì** per consentire all'Editor del Registro di sistema di apportare modifiche al dispositivo.</span><span class="sxs-lookup"><span data-stu-id="82a18-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="82a18-112">Nell'Editor del Registro di sistema aggiungi un valore DWORD **EnableADAL** con un'impostazione pari a **0** in HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="82a18-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="82a18-113">Per ulteriori informazioni, vedere Problemi di connessione nell'accesso dopo l'aggiornamento a [Office 2016 build 16.0.7967 in Windows 10.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)</span><span class="sxs-lookup"><span data-stu-id="82a18-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>