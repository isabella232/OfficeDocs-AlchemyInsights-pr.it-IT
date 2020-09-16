---
title: Fissaggio delle app di Microsoft 365 Impossibile trovare il messaggio associato alle licenze di Office
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
- "3421"
- "9001426"
ms.openlocfilehash: bd127d6287b4438f6105a6158abdbd5b964b7e70
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747699"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="6fc80-102">Risoluzione delle app di Microsoft 365 "Impossibile trovare il messaggio relativo alle licenze di Office"</span><span class="sxs-lookup"><span data-stu-id="6fc80-102">Fixing the Microsoft 365 apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="6fc80-103">Se viene visualizzato questo messaggio, provare a eseguire le operazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="6fc80-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="6fc80-104">Controllare il firewall, il software antivirus e le impostazioni proxy per confermare che non bloccano l'accesso a Internet alle app Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="6fc80-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="6fc80-105">Vedere gli [intervalli di indirizzi IP e URL di Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="6fc80-105">See [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="6fc80-106">Rimuovere e [riassegnare la licenza di Office](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) per l'utente in questione.</span><span class="sxs-lookup"><span data-stu-id="6fc80-106">Remove and [reassign the Office license](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="6fc80-107">Aprire un'app di Office e [disconnettersi](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) da tutti gli account utente esistenti.</span><span class="sxs-lookup"><span data-stu-id="6fc80-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="6fc80-108">Passare a impostazioni di Windows **> account**  >  **& di posta elettronica**e rimuovere tutti gli account di lavoro, ad eccezione dell'account danneggiato.</span><span class="sxs-lookup"><span data-stu-id="6fc80-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="6fc80-109">Passare a impostazioni di Windows > **account**di  >  **accesso al lavoro o all'Istituto di istruzione**e disconnettere tutti gli account di lavoro ad eccezione dell'account danneggiato.</span><span class="sxs-lookup"><span data-stu-id="6fc80-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="6fc80-110">Reimposta lo stato di attivazione di Office.</span><span class="sxs-lookup"><span data-stu-id="6fc80-110">Reset the Office activation state.</span></span> <span data-ttu-id="6fc80-111">[Procedura](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state)</span><span class="sxs-lookup"><span data-stu-id="6fc80-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="6fc80-112">[Accedere](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) utilizzando l'account utente in questione.</span><span class="sxs-lookup"><span data-stu-id="6fc80-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="6fc80-113">Per ulteriori soluzioni per la risoluzione dei problemi, vedere [errori di attivazione e di prodotto senza licenza in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="6fc80-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>