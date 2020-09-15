---
title: Risolvere l'errore L'applicazione non è stata rilevata
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000171"
- "1712"
ms.openlocfilehash: 498c2ec78bc9f4a7bc7d77d12b488be2cf0bf79a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666982"
---
# <a name="mitigate-the-application-was-not-detected-error"></a><span data-ttu-id="df8ec-102">Risolvere l'errore "L'applicazione non è stata rilevata"</span><span class="sxs-lookup"><span data-stu-id="df8ec-102">Mitigate "The application was not detected" error</span></span>

<span data-ttu-id="df8ec-103">L'errore di installazione dell'app "L'applicazione non è stata rilevata dopo il completamento dell'installazione" segnalato da Intune potrebbe comparire in tutte le principali piattaforme di sistemi operativi (Windows, iOS e Android).</span><span class="sxs-lookup"><span data-stu-id="df8ec-103">The app installation error, “The application was not detected after installation completed successfully,” reported by Intune, may occur on all major OS platforms (Windows, iOS and Android).</span></span>

<span data-ttu-id="df8ec-104">Gli scenari più comuni che generano questo errore includono:</span><span class="sxs-lookup"><span data-stu-id="df8ec-104">The most common scenarios that generate this error include:</span></span>

- <span data-ttu-id="df8ec-105">L'app è stata aggiornata all'esterno di Intune (da un App Store di terze parti) dopo la distribuzione iniziale.</span><span class="sxs-lookup"><span data-stu-id="df8ec-105">The app has been updated outside of Intune (from a third-party app store) after the initial deployment.</span></span> <span data-ttu-id="df8ec-106">Ad esempio, alcune applicazioni come Google Chrome potrebbero eseguire gli aggiornamenti automatici.</span><span class="sxs-lookup"><span data-stu-id="df8ec-106">For example some applications such as Google Chrome may perform auto updates.</span></span>
- <span data-ttu-id="df8ec-107">Dopo l'installazione iniziale, un utente ha disinstallato l'app.</span><span class="sxs-lookup"><span data-stu-id="df8ec-107">A user has uninstalled the app after the initial install.</span></span>

<span data-ttu-id="df8ec-108">Per ovviare a questo problema, eseguire prima di tutto una revisione dei dispositivi interessati per determinare lo scenario in cui si verifica l'errore.</span><span class="sxs-lookup"><span data-stu-id="df8ec-108">To mitigate this issue, first perform a review of the affected devices to determine the scenario in which the error occurs.</span></span>

- <span data-ttu-id="df8ec-109">Se l'app è stata aggiornata all'esterno di Intune, la distribuzione dell'app potrebbe essere stata impostata per ignorare la versione dell'applicazione.</span><span class="sxs-lookup"><span data-stu-id="df8ec-109">If the app has been updated outside of Intune, the app deployment can be set to ignore the application version.</span></span> <span data-ttu-id="df8ec-110">A questo scopo, in **Configurazione dell'app > Informazioni sull'app** impostare **Ignora la versione dell'app** su **Sì**.</span><span class="sxs-lookup"><span data-stu-id="df8ec-110">To do so, under **App Configuration > App Information**, set **Ignore App** version to **Yes**.</span></span>
- <span data-ttu-id="df8ec-111">Durante l'assegnazione del client, potrebbe essere opportuno distribuire l'applicazione come "obbligatoria" e assicurarsi che venga distribuita l'ultima versione.</span><span class="sxs-lookup"><span data-stu-id="df8ec-111">When targeting the client, it may be appropriate to deploy the application as “required,” and to ensure that the latest version is deployed.</span></span>
- <span data-ttu-id="df8ec-112">In alternativa, nella piattaforma iOS è possibile usare la funzionalità di **aggiornamento automatico** associata al Volume Purchase Program di Apple, che può essere configurata per l'aggiornamento automatico alle nuove versioni di applicazioni quando diventano disponibili.</span><span class="sxs-lookup"><span data-stu-id="df8ec-112">Alternatively, on the iOS platform, it is possible to use the **autoupdate** functionality associated with the Apple Volume Purchase Program, which can be configured to automatically update to new application versions as they become available.</span></span>

<span data-ttu-id="df8ec-113">Per altre informazioni sulla risoluzione dei problemi di installazione delle app, vedere [Risoluzione dei problemi di installazione delle app](https://docs.microsoft.com/intune/troubleshoot-app-install).</span><span class="sxs-lookup"><span data-stu-id="df8ec-113">For more information about troubleshooting app installation issues, please see [Troubleshoot app installation issues](https://docs.microsoft.com/intune/troubleshoot-app-install).</span></span>
