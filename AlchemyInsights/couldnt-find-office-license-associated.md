---
title: Correzione delle app di Microsoft 365 Impossibile trovare il messaggio associato alle licenze di Office
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
- "3421"
- "9001426"
ms.openlocfilehash: 1d717fce77de2f55dfc983d42b7f8d46a8c212e7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816492"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="72b74-102">Correzione del messaggio "Impossibile trovare licenze di Office associate" per le app di Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="72b74-102">Fixing the Microsoft 365 apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="72b74-103">Se viene visualizzato questo messaggio, provare a eseguire le operazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="72b74-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="72b74-104">Controllare le impostazioni del firewall, del software antivirus e del proxy per verificare che non blocchino l'accesso a Internet alle app di Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="72b74-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="72b74-105">Vedere URL e intervalli di indirizzi [IP di Microsoft 365.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="72b74-105">See [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="72b74-106">Rimuovere e [riassegnare la licenza di Office per](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) l'utente interessato.</span><span class="sxs-lookup"><span data-stu-id="72b74-106">Remove and [reassign the Office license](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="72b74-107">Aprire un'app di Office [e disconnettersi](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) da qualsiasi account utente esistente.</span><span class="sxs-lookup"><span data-stu-id="72b74-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="72b74-108">Vai a Impostazioni di Windows > **account e-mail**& account e rimuovi tutti gli account di lavoro ad  >  eccezione dell'account interessato.</span><span class="sxs-lookup"><span data-stu-id="72b74-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="72b74-109">Vai a Impostazioni di Windows > **account Accedi** all'istituto di istruzione o all'istituto di istruzione e disconnetti tutti gli account di lavoro ad eccezione  >  dell'account interessato.</span><span class="sxs-lookup"><span data-stu-id="72b74-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="72b74-110">Reimposta lo stato di attivazione di Office.</span><span class="sxs-lookup"><span data-stu-id="72b74-110">Reset the Office activation state.</span></span> <span data-ttu-id="72b74-111">[Procedura](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state)</span><span class="sxs-lookup"><span data-stu-id="72b74-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="72b74-112">[Accedi con](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) l'account utente interessato.</span><span class="sxs-lookup"><span data-stu-id="72b74-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="72b74-113">Per ulteriori soluzioni di risoluzione dei problemi, vedere Errori di attivazione e prodotti senza [licenza in Office.](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)</span><span class="sxs-lookup"><span data-stu-id="72b74-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>