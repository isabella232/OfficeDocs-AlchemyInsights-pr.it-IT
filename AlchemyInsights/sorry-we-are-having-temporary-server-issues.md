---
title: Fixing Microsoft 365 apps Sorry, we are having temporary server issues message
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
- "3420"
- "9001430"
ms.openlocfilehash: 0adf1d66869051b9dd8290ef3466ef9b13aa2d41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835275"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="ec4a2-102">Correzione del messaggio "Ci sono problemi temporanei del server" per le app di Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="ec4a2-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="ec4a2-103">Se viene visualizzato questo messaggio, provare a eseguire le operazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="ec4a2-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="ec4a2-104">Controllare le impostazioni del firewall, del software antivirus e del proxy per verificare che non blocchino l'accesso a Internet alle app di Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="ec4a2-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="ec4a2-105">Vedere [URL e intervalli di indirizzi IP.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="ec4a2-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="ec4a2-106">Go to **Start**  >  **Run**, and then type **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="ec4a2-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="ec4a2-107">Verificare che tutti i servizi seguenti siano in esecuzione:</span><span class="sxs-lookup"><span data-stu-id="ec4a2-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="ec4a2-108">Configurazione automatica dei dispositivi connessi in rete</span><span class="sxs-lookup"><span data-stu-id="ec4a2-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="ec4a2-109">Servizio elenco di rete</span><span class="sxs-lookup"><span data-stu-id="ec4a2-109">Network List Service</span></span>
    - <span data-ttu-id="ec4a2-110">Sensibilizzazione percorso di rete</span><span class="sxs-lookup"><span data-stu-id="ec4a2-110">Network Location Awareness</span></span>
    - <span data-ttu-id="ec4a2-111">Registro eventi di Windows</span><span class="sxs-lookup"><span data-stu-id="ec4a2-111">Windows Event Log</span></span>

<span data-ttu-id="ec4a2-112">Se uno di questi servizi non è in esecuzione, provare ad avviarlo.</span><span class="sxs-lookup"><span data-stu-id="ec4a2-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="ec4a2-113">Se si verifica un problema durante l'avvio del servizio, eseguire il comando seguente aprendo un prompt dei comandi con autorizzazioni elevate:</span><span class="sxs-lookup"><span data-stu-id="ec4a2-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="ec4a2-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="ec4a2-114">**sfc /scannow**</span></span>

<span data-ttu-id="ec4a2-115">Al termine del comando, riavviare il computer.</span><span class="sxs-lookup"><span data-stu-id="ec4a2-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="ec4a2-116">Per informazioni dettagliate, vedere ["Spiacenti, non è possibile connettersi al tuo account. Riprovare più tardi" quando si attiva](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="ec4a2-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>