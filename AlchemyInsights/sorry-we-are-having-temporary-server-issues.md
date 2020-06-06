---
title: Risoluzione dei problemi relativi alle app di Microsoft 365, è stato riscontrato un messaggio temporaneo relativo ai server
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: 6db04a437de8e50af349b5c690791981ae872f14
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582707"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="40434-102">Risoluzione dei problemi relativi alle app Microsoft 365 "dispiaciuti del problema del server temporaneo"</span><span class="sxs-lookup"><span data-stu-id="40434-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="40434-103">Se viene visualizzato questo messaggio, provare a eseguire le operazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="40434-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="40434-104">Controllare il firewall, il software antivirus e le impostazioni proxy per confermare che non bloccano l'accesso a Internet alle app Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="40434-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="40434-105">Vedere [URL e intervalli di indirizzi IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="40434-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="40434-106">Andare a **Start**  >  **Run**e quindi digitare **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="40434-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="40434-107">Verificare che i seguenti servizi siano in esecuzione:</span><span class="sxs-lookup"><span data-stu-id="40434-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="40434-108">Configurazione automatica di dispositivi connessi alla rete</span><span class="sxs-lookup"><span data-stu-id="40434-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="40434-109">Servizio elenco di rete</span><span class="sxs-lookup"><span data-stu-id="40434-109">Network List Service</span></span>
    - <span data-ttu-id="40434-110">Consapevolezza del percorso di rete</span><span class="sxs-lookup"><span data-stu-id="40434-110">Network Location Awareness</span></span>
    - <span data-ttu-id="40434-111">Registro eventi di Windows</span><span class="sxs-lookup"><span data-stu-id="40434-111">Windows Event Log</span></span>

<span data-ttu-id="40434-112">Se uno di questi servizi non è in esecuzione, provare a avviarlo.</span><span class="sxs-lookup"><span data-stu-id="40434-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="40434-113">In caso di problemi durante l'avvio del servizio, eseguire il comando riportato di seguito aprendo un prompt dei comandi con autorizzazioni elevate:</span><span class="sxs-lookup"><span data-stu-id="40434-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="40434-114">**SFC/scannow**</span><span class="sxs-lookup"><span data-stu-id="40434-114">**sfc /scannow**</span></span>

<span data-ttu-id="40434-115">Al termine del comando, riavviare il computer.</span><span class="sxs-lookup"><span data-stu-id="40434-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="40434-116">Per informazioni dettagliate, vedere [la sezione "spiacenti, non è possibile connettersi al proprio account. Si prega di riprovare più tardi "errore quando si attiva](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="40434-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>