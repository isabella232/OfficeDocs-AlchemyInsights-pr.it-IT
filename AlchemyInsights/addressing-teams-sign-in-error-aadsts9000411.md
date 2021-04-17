---
title: "Risolvere l'errore di accesso AADSTS9000411 in Teams "
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: 7b0e90e3fea716df649ec906ad8b3008386684be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821991"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a><span data-ttu-id="043d8-102">Risolvere l'errore di accesso AADSTS9000411 in Teams </span><span class="sxs-lookup"><span data-stu-id="043d8-102">Addressing Teams sign-in error AADSTS9000411</span></span>

<span data-ttu-id="043d8-103">Quando si esegue l'accesso a Microsoft Teams, è possibile che venga visualizzato il messaggio di errore: **Si è verificato un problema di accesso di tipo AADSTS9000411: la richiesta non è stata formattata correttamente. Il parametro "login_hint" è stato duplicato.**</span><span class="sxs-lookup"><span data-stu-id="043d8-103">When signing in to Microsoft Teams, you may receive the error: **Sorry, but we're having trouble with signing you in AADSTS9000411: The request is not properly formatted. The parameter "login_hint" is duplicated.**</span></span>

<span data-ttu-id="043d8-104">Per risolvere il problema, verificare che i client di Microsoft Teams siano aggiornati.</span><span class="sxs-lookup"><span data-stu-id="043d8-104">To address this issue, please ensure your Microsoft Teams clients are updated.</span></span> <span data-ttu-id="043d8-105">Per altre informazioni sull'aggiornamento del client, vedere [Aggiornare Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="043d8-105">For more information on updating your client, see [Update Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

<span data-ttu-id="043d8-106">Se non è possibile aggiornare il client per qualche motivo, disconnettendo il client sarà possibile eliminare la maggior parte dei dati memorizzati nella cache.</span><span class="sxs-lookup"><span data-stu-id="043d8-106">If you cannot update your client for some reason, logging off the client will clear most cached data.</span></span> <span data-ttu-id="043d8-107">Tuttavia, se si verificano ancora problemi dopo la disconnessione/connessione, chiudere Teams e cancellare la cache del client eseguendo le operazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="043d8-107">However, if you still have issues after logoff/logon, quit Teams and please clear your client cache by doing the following:</span></span>
1. <span data-ttu-id="043d8-108">Chiudere Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="043d8-108">Close Microsoft Teams.</span></span>
2. <span data-ttu-id="043d8-109">Passare a: %appdata%\microsoft\teams e cancellare tutti i file.</span><span class="sxs-lookup"><span data-stu-id="043d8-109">Go to: %appdata%\microsoft\teams and delete all the files.</span></span>
3. <span data-ttu-id="043d8-110">Riaprire Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="043d8-110">Reopen Microsoft Teams.</span></span>
