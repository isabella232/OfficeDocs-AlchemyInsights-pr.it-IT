---
title: 'Problema di attivazione: non è possibile connettersi in questo momento'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 84e3a7700558ad8a5fad5b7ded6354fe8736e0f7
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/27/2019
ms.locfileid: "39628246"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="b14c9-102">Risoluzione delle app di Office "non è possibile connettersi subito" messaggio</span><span class="sxs-lookup"><span data-stu-id="b14c9-102">Fixing the Office apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="b14c9-103">Se viene visualizzato questo messaggio, provare a eseguire le operazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="b14c9-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="b14c9-104">Controllare il firewall, il software antivirus e le impostazioni proxy per confermare che non bloccano l'accesso a Internet alle app di Office.</span><span class="sxs-lookup"><span data-stu-id="b14c9-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="b14c9-105">Vedere gli [intervalli di indirizzi IP e URL di Office 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="b14c9-105">See [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="b14c9-106">Andare a **Start** > **Run**e quindi digitare **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="b14c9-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="b14c9-107">Verificare che i seguenti servizi siano in esecuzione:</span><span class="sxs-lookup"><span data-stu-id="b14c9-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="b14c9-108">Configurazione automatica di dispositivi connessi alla rete</span><span class="sxs-lookup"><span data-stu-id="b14c9-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="b14c9-109">Servizio elenco di rete</span><span class="sxs-lookup"><span data-stu-id="b14c9-109">Network List Service</span></span>
    - <span data-ttu-id="b14c9-110">Consapevolezza del percorso di rete</span><span class="sxs-lookup"><span data-stu-id="b14c9-110">Network Location Awareness</span></span>
    - <span data-ttu-id="b14c9-111">Registro eventi di Windows</span><span class="sxs-lookup"><span data-stu-id="b14c9-111">Windows Event Log</span></span>

<span data-ttu-id="b14c9-112">Se uno di questi servizi non è in esecuzione, provare a avviarlo.</span><span class="sxs-lookup"><span data-stu-id="b14c9-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="b14c9-113">In caso di problemi durante l'avvio del servizio, eseguire il comando riportato di seguito aprendo un prompt dei comandi con autorizzazioni elevate:</span><span class="sxs-lookup"><span data-stu-id="b14c9-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="b14c9-114">**SFC/scannow**</span><span class="sxs-lookup"><span data-stu-id="b14c9-114">**sfc /scannow**</span></span>

<span data-ttu-id="b14c9-115">Al termine del comando, riavviare il computer.</span><span class="sxs-lookup"><span data-stu-id="b14c9-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="b14c9-116">Per informazioni dettagliate, vedere [la sezione "spiacenti, non è possibile connettersi al proprio account. Si prega di riprovare più tardi quando si attiva Office da Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="b14c9-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>