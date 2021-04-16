---
title: 'Problema di attivazione: al momento non è possibile connettersi'
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
- "3408"
- "9001423"
ms.openlocfilehash: 2dd3c97bb85254215b13ee8a1222941c0492b204
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51806446"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="5bbb1-102">Correzione del messaggio "Non è possibile connettersi subito" alle app di Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="5bbb1-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="5bbb1-103">Se viene visualizzato questo messaggio, provare a eseguire le operazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="5bbb1-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="5bbb1-104">Controllare le impostazioni del firewall, del software antivirus e del proxy per verificare che non blocchino l'accesso a Internet alle app di Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="5bbb1-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="5bbb1-105">Vedere [URL Microsoft e intervalli di indirizzi IP.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="5bbb1-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="5bbb1-106">Go to **Start**  >  **Run**, and then type **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="5bbb1-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="5bbb1-107">Verificare che tutti i servizi seguenti siano in esecuzione:</span><span class="sxs-lookup"><span data-stu-id="5bbb1-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="5bbb1-108">Configurazione automatica dei dispositivi connessi in rete</span><span class="sxs-lookup"><span data-stu-id="5bbb1-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="5bbb1-109">Servizio elenco di rete</span><span class="sxs-lookup"><span data-stu-id="5bbb1-109">Network List Service</span></span>
    - <span data-ttu-id="5bbb1-110">Sensibilizzazione percorso di rete</span><span class="sxs-lookup"><span data-stu-id="5bbb1-110">Network Location Awareness</span></span>
    - <span data-ttu-id="5bbb1-111">Registro eventi di Windows</span><span class="sxs-lookup"><span data-stu-id="5bbb1-111">Windows Event Log</span></span>

<span data-ttu-id="5bbb1-112">Se uno di questi servizi non è in esecuzione, provare ad avviarlo.</span><span class="sxs-lookup"><span data-stu-id="5bbb1-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="5bbb1-113">Se si verifica un problema durante l'avvio del servizio, eseguire il comando seguente aprendo un prompt dei comandi con autorizzazioni elevate:</span><span class="sxs-lookup"><span data-stu-id="5bbb1-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="5bbb1-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="5bbb1-114">**sfc /scannow**</span></span>

<span data-ttu-id="5bbb1-115">Al termine del comando, riavviare il computer.</span><span class="sxs-lookup"><span data-stu-id="5bbb1-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="5bbb1-116">Per informazioni dettagliate, vedere ["Spiacenti, non è possibile connettersi al tuo account. Riprovare più tardi" quando si attiva Office da Microsoft 365.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)</span><span class="sxs-lookup"><span data-stu-id="5bbb1-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>