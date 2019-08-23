---
title: Problemi di accesso alle app di Office
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
- "2574"
ms.openlocfilehash: 3622a3408b25b43090e9414ae5ffcfc2760264ee
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938254"
---
# <a name="issues-signing-in-to-office-apps"></a><span data-ttu-id="c4e20-102">Problemi di accesso alle app di Office</span><span class="sxs-lookup"><span data-stu-id="c4e20-102">Issues signing in to Office apps</span></span>

<span data-ttu-id="c4e20-103">Per risolvere i problemi di accesso con le app di Office, provare a eseguire le operazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="c4e20-103">To fix sign-in issues with Office apps, try the following:</span></span>

- <span data-ttu-id="c4e20-104">Rimuovere tutti gli account di lavoro, ad eccezione dell'account danneggiato, utilizzando le impostazioni di Windows > **accedere al lavoro o all'Istituto di istruzione**.</span><span class="sxs-lookup"><span data-stu-id="c4e20-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="c4e20-105">[Cancellare le credenziali di Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) utilizzando Gestione credenziali di Windows.</span><span class="sxs-lookup"><span data-stu-id="c4e20-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="c4e20-106">**Nota:** I percorsi del registro di sistema per Office 2016 sono stati modificati in 16,0.</span><span class="sxs-lookup"><span data-stu-id="c4e20-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="c4e20-107">(Es: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="c4e20-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="c4e20-108">Aprire un'app di Office, scegliere**Esci dall'\*\*\*\*account** >  **file** > . Accedere quindi utilizzando un account utente con una licenza valida.</span><span class="sxs-lookup"><span data-stu-id="c4e20-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="c4e20-109">Per informazioni dettagliate, vedere [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="c4e20-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="c4e20-110">Per Mac, vedere [Impossibile accedere a un'app di Office 2016 per Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="c4e20-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>
- <span data-ttu-id="c4e20-111">Se si verificano errori durante la connessione a Office 365 con Office 2013, abilitare l'autenticazione moderna per il client di Office.</span><span class="sxs-lookup"><span data-stu-id="c4e20-111">If the errors occurs while connecting to Office 365 using Office 2013, enable modern authentication for Office client.</span></span>

<span data-ttu-id="c4e20-112">Per ulteriori informazioni, vedere:</span><span class="sxs-lookup"><span data-stu-id="c4e20-112">For more information, see:</span></span>
- [<span data-ttu-id="c4e20-113">Non è possibile accedere a Office 365, Azure o Intune</span><span class="sxs-lookup"><span data-stu-id="c4e20-113">You can't sign in to Office 365, Azure, or Intune</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [<span data-ttu-id="c4e20-114">Problemi di connessione in accesso dopo l'aggiornamento a Office 2016 Build 16.0.7967 in Windows 10</span><span class="sxs-lookup"><span data-stu-id="c4e20-114">Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10</span></span>](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- [<span data-ttu-id="c4e20-115">"Spiacenti, un altro account dell'organizzazione è già stato eseguito l'accesso al computer" in Office</span><span class="sxs-lookup"><span data-stu-id="c4e20-115">"Sorry, another account from your organization is already signed in on this computer" in Office</span></span>](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [<span data-ttu-id="c4e20-116">Risoluzione dei problemi di accesso con l'autenticazione moderna di Office quando si utilizzano ADFS</span><span class="sxs-lookup"><span data-stu-id="c4e20-116">Troubleshoot sign-in issues with Office modern authentication when you use ADFS</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)