---
title: Exchange PowerShell e deprecazione dell'autenticazione di base
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
- "3500011"
- "4577"
ms.openlocfilehash: 01938a59b53ccf8b7867ed9c256e141205d31dff
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813476"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="744df-102">Exchange PowerShell e deprecazione dell'autenticazione di base</span><span class="sxs-lookup"><span data-stu-id="744df-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="744df-103">Per le informazioni più recenti riguardanti le modalità di connessione Exchange Online PowerShell senza l'uso dell'autenticazione di base, [fare clic qui](https://aka.ms/exops-docs).</span><span class="sxs-lookup"><span data-stu-id="744df-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/exops-docs).</span></span> <span data-ttu-id="744df-104">Il modulo di PowerShell V2 non usa l'autenticazione di base.</span><span class="sxs-lookup"><span data-stu-id="744df-104">The PowerShell V2 module does not use basic authentication.</span></span>

<span data-ttu-id="744df-105">Tenere presente che l'autenticazione di base deve comunque essere abilitata nel computer client.</span><span class="sxs-lookup"><span data-stu-id="744df-105">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="744df-106">Il nuovo modulo PowerShell V2 usa l'autenticazione moderna per stabilire una connessione per l'abilitazione di tutti i cmdlet V2 basati su REST.</span><span class="sxs-lookup"><span data-stu-id="744df-106">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="744df-107">Oltre ai cmdlet V2, consente anche di accedere ai cmdlet di PowerShell remoto (RPS) meno recenti, per cui è necessario stabilire una sessione PowerShell remota.</span><span class="sxs-lookup"><span data-stu-id="744df-107">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="744df-108">Per stabilire una sessione RPS in un computer Windows, è necessario abilitare WinRM BasicAuth nel computer client anche se il modulo usa il meccanismo di autenticazione moderna per l'autenticazione nel servizio.</span><span class="sxs-lookup"><span data-stu-id="744df-108">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="744df-109">La pipeline di autenticazione di base WinRM consente di trasportare i token di autenticazione moderna.</span><span class="sxs-lookup"><span data-stu-id="744df-109">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="744df-110">Se l'autenticazione di base WinRM è disabilitata nel computer client, i nuovi cmdlet V2 continueranno a funzionare, ma i cmdlet RPS meno recenti non funzioneranno più.</span><span class="sxs-lookup"><span data-stu-id="744df-110">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
