---
title: Risoluzione delle app di Office l'account è in un messaggio di stato non valido
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: e591c56dd207a5bcb3979be3f66052121100b162
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/27/2019
ms.locfileid: "41969561"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a><span data-ttu-id="4af04-102">Errore di correzione delle app di Office "l'account è in uno stato non valido"</span><span class="sxs-lookup"><span data-stu-id="4af04-102">Fixing the Office apps "Your account is in a bad state" error</span></span>

<span data-ttu-id="4af04-103">Per correggere l'errore, provare a eseguire le opzioni seguenti nel computer in questione:</span><span class="sxs-lookup"><span data-stu-id="4af04-103">To fix this error, try the following options on the affected computer:</span></span>

- <span data-ttu-id="4af04-104">Aprire un'app di Office, \*\*\*\* > Selezionare l'**account** > **di accesso al file fuori da tutti gli account**.</span><span class="sxs-lookup"><span data-stu-id="4af04-104">Open an Office app, select **File** > **Account** > **Sign Out of all accounts**.</span></span> <span data-ttu-id="4af04-105">Eseguire di nuovo l'accesso utilizzando un account utente con una licenza valida.</span><span class="sxs-lookup"><span data-stu-id="4af04-105">Sign in again using a user account with a valid license.</span></span> <span data-ttu-id="4af04-106">Per informazioni dettagliate, vedere [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="4af04-106">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="4af04-107">[Cancellare le credenziali di Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) utilizzando Gestione credenziali di Windows.</span><span class="sxs-lookup"><span data-stu-id="4af04-107">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br>
  <span data-ttu-id="4af04-108">**Nota:** I percorsi del registro di sistema per Office 2016 sono stati modificati in 16,0.</span><span class="sxs-lookup"><span data-stu-id="4af04-108">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="4af04-109">Ad esempio, \Software\Microsoft\Office\16.0\Common\Identity</span><span class="sxs-lookup"><span data-stu-id="4af04-109">For example, \Software\Microsoft\Office\16.0\Common\Identity</span></span>\
- <span data-ttu-id="4af04-110">Nel computer in questione, impostare EnableADAL = 0 eseguendo la procedura seguente:</span><span class="sxs-lookup"><span data-stu-id="4af04-110">On the affected computer, set the EnableADAL = 0 using the following steps:</span></span>  
     1. <span data-ttu-id="4af04-111">Fare clic con il pulsante destro del mouse su Windows e scegliere **Esegui**.</span><span class="sxs-lookup"><span data-stu-id="4af04-111">Right-click the Windows button and select **Run**.</span></span> <span data-ttu-id="4af04-112">Nella casella **Apri** Digitare **Regedit**e quindi fare clic su **OK**.</span><span class="sxs-lookup"><span data-stu-id="4af04-112">In the **Open** box, type **regedit**, and then select **OK**.</span></span>
     2. <span data-ttu-id="4af04-113">Selezionare **Sì** quando viene richiesto di consentire all'editor del registro di sistema di apportare modifiche al dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4af04-113">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="4af04-114">Nell'editor del registro di sistema, aggiungere un valore DWORD di EnableADAL con un'impostazione pari a 0 in HKEY_CURRENT_USER \Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="4af04-114">In the Registry Editor, add a DWORD value of EnableADAL with a setting of 0 under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>
- <span data-ttu-id="4af04-115">Se si verifica un errore durante la connessione a Office 365 con Office 2013, [abilitare l'autenticazione moderna](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) per il client di Office.</span><span class="sxs-lookup"><span data-stu-id="4af04-115">If the error occurs while connecting to Office 365 using Office 2013, [enable modern authentication](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) for the Office client.</span></span>

<span data-ttu-id="4af04-116">Per ulteriori informazioni, vedere [come risolvere i problemi relativi alle app non browser che non sono in grado di accedere a Office 365, Azure o Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span><span class="sxs-lookup"><span data-stu-id="4af04-116">For more information, see [How to troubleshoot non-browser apps that can't sign in to Office 365, Azure, or Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span></span>

