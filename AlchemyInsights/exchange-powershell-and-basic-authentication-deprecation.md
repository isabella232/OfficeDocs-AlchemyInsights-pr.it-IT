---
title: Exchange PowerShell e deprecazione dell'autenticazione di base
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 24d59860732b42e8d62da8c1a8c37f2018a0d126
ms.sourcegitcommit: 264b782ac2fba8ffd84524180dc4f7d60b45e9a4
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 05/04/2020
ms.locfileid: "44015693"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="922a2-102">Exchange PowerShell e deprecazione dell'autenticazione di base</span><span class="sxs-lookup"><span data-stu-id="922a2-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="922a2-103">Per le informazioni più recenti riguardanti le modalità di connessione Exchange Online PowerShell senza l'uso dell'autenticazione di base, [fare clic qui](https://aka.ms/psbasicauth).</span><span class="sxs-lookup"><span data-stu-id="922a2-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/psbasicauth).</span></span>

<span data-ttu-id="922a2-104">Tenere presente che l'autenticazione di base deve comunque essere abilitata nel computer client.</span><span class="sxs-lookup"><span data-stu-id="922a2-104">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="922a2-105">Il nuovo modulo PowerShell V2 usa l'autenticazione moderna per stabilire una connessione per l'abilitazione di tutti i cmdlet V2 basati su REST.</span><span class="sxs-lookup"><span data-stu-id="922a2-105">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="922a2-106">Oltre ai cmdlet V2, consente anche di accedere ai cmdlet di PowerShell remoto (RPS) meno recenti, per cui è necessario stabilire una sessione PowerShell remota.</span><span class="sxs-lookup"><span data-stu-id="922a2-106">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="922a2-107">Per stabilire una sessione RPS in un computer Windows, è necessario abilitare WinRM BasicAuth nel computer client anche se il modulo usa il meccanismo di autenticazione moderna per l'autenticazione nel servizio.</span><span class="sxs-lookup"><span data-stu-id="922a2-107">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="922a2-108">La pipeline di autenticazione di base WinRM consente di trasportare i token di autenticazione moderna.</span><span class="sxs-lookup"><span data-stu-id="922a2-108">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="922a2-109">Se l'autenticazione di base WinRM è disabilitata nel computer client, i nuovi cmdlet V2 continueranno a funzionare, ma i cmdlet RPS meno recenti non funzioneranno più.</span><span class="sxs-lookup"><span data-stu-id="922a2-109">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
