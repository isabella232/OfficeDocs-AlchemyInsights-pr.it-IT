---
title: 'Problema di attivazione: non è possibile connettersi in questo momento'
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
- "3408"
- "9001423"
ms.openlocfilehash: 24fe9910d1715b4f5f7d8d06b1d1344d4b8675bc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725987"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="44040-102">Risoluzione delle app Microsoft 365 "non è possibile connettersi in questo momento" messaggio</span><span class="sxs-lookup"><span data-stu-id="44040-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="44040-103">Se viene visualizzato questo messaggio, provare a eseguire le operazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="44040-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="44040-104">Controllare il firewall, il software antivirus e le impostazioni proxy per confermare che non bloccano l'accesso a Internet alle app Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="44040-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="44040-105">Vedere gli [intervalli di indirizzi IP e URL Microsoft](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="44040-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="44040-106">Andare a **Start**  >  **Run**e quindi digitare **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="44040-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="44040-107">Verificare che i seguenti servizi siano in esecuzione:</span><span class="sxs-lookup"><span data-stu-id="44040-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="44040-108">Configurazione automatica di dispositivi connessi alla rete</span><span class="sxs-lookup"><span data-stu-id="44040-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="44040-109">Servizio elenco di rete</span><span class="sxs-lookup"><span data-stu-id="44040-109">Network List Service</span></span>
    - <span data-ttu-id="44040-110">Consapevolezza del percorso di rete</span><span class="sxs-lookup"><span data-stu-id="44040-110">Network Location Awareness</span></span>
    - <span data-ttu-id="44040-111">Registro eventi di Windows</span><span class="sxs-lookup"><span data-stu-id="44040-111">Windows Event Log</span></span>

<span data-ttu-id="44040-112">Se uno di questi servizi non è in esecuzione, provare a avviarlo.</span><span class="sxs-lookup"><span data-stu-id="44040-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="44040-113">In caso di problemi durante l'avvio del servizio, eseguire il comando riportato di seguito aprendo un prompt dei comandi con autorizzazioni elevate:</span><span class="sxs-lookup"><span data-stu-id="44040-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="44040-114">**SFC/scannow**</span><span class="sxs-lookup"><span data-stu-id="44040-114">**sfc /scannow**</span></span>

<span data-ttu-id="44040-115">Al termine del comando, riavviare il computer.</span><span class="sxs-lookup"><span data-stu-id="44040-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="44040-116">Per informazioni dettagliate, vedere [la sezione "spiacenti, non è possibile connettersi al proprio account. Si prega di riprovare più tardi quando si attiva Office da Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="44040-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>