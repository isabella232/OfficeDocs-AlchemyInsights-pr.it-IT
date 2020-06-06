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
- "2560"
ms.openlocfilehash: e4f2fea5c2f368ae240614ee1f7bc729338dd75d
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579941"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a><span data-ttu-id="ac096-102">Risoluzione delle app Microsoft 365 "spiacenti, un altro account dell'organizzazione è già stato firmato in" messaggio</span><span class="sxs-lookup"><span data-stu-id="ac096-102">Fixing the Microsoft 365 apps "Sorry, another account from your organization is already signed in" message</span></span>

<span data-ttu-id="ac096-103">Per risolvere il problema, provare a eseguire le operazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="ac096-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="ac096-104">Rimuovere tutti gli account di lavoro, ad eccezione dell'account danneggiato, utilizzando le impostazioni di Windows > **accedere al lavoro o all'Istituto di istruzione**.</span><span class="sxs-lookup"><span data-stu-id="ac096-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="ac096-105">[Cancellare le credenziali di Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) utilizzando Gestione credenziali di Windows.</span><span class="sxs-lookup"><span data-stu-id="ac096-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="ac096-106">**Nota:** I percorsi del registro di sistema per Office 2016 sono stati modificati in 16,0.</span><span class="sxs-lookup"><span data-stu-id="ac096-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="ac096-107">(Es: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="ac096-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="ac096-108">Aprire un'app di Office, **File**scegliere  >  **Account**  >  **Esci dall'** account file. Accedere quindi utilizzando un account utente con una licenza valida.</span><span class="sxs-lookup"><span data-stu-id="ac096-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="ac096-109">Per informazioni dettagliate, vedere [Account in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="ac096-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="ac096-110">Per Mac, vedere [Non è possibile accedere a un'app di Office 2016 per Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="ac096-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>

<span data-ttu-id="ac096-111">Per ulteriori informazioni, vedere [la sezione "spiacenti, un altro account dell'organizzazione è già stato eseguito l'accesso a questo computer" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span><span class="sxs-lookup"><span data-stu-id="ac096-111">For more information, see ["Sorry, another account from your organization is already signed in on this computer" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span></span>