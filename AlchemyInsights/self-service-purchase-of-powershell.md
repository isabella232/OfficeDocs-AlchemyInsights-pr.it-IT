---
title: Acquisto in modalità self-service di PowerShell
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
- "9001212"
- "3516"
ms.openlocfilehash: e6cc504ebef19cbe78f576d9b207fe2d951d0ef5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47739974"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="4de38-102">Acquisto in modalità self-service di PowerShell</span><span class="sxs-lookup"><span data-stu-id="4de38-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="4de38-103">Per utilizzare il modulo di MSCommerce PowerShell, è necessario installarlo su un dispositivo Windows 10 con TLS 1,2 (autorizzazioni di amministratore locale necessarie).</span><span class="sxs-lookup"><span data-stu-id="4de38-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="4de38-104">Importare e connettersi al modulo MSCommerce.</span><span class="sxs-lookup"><span data-stu-id="4de38-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="4de38-105">Quando viene richiesto di eseguire l'accesso, sarà necessario utilizzare le credenziali del ruolo di amministratore globale o di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="4de38-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="4de38-106">Se non si dispone di TLS 1,2, è possibile che venga visualizzato il seguente messaggio di errore quando si tenta di ottenere o aggiornare il criterio:</span><span class="sxs-lookup"><span data-stu-id="4de38-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="4de38-107">*ErrorMessage-la connessione sottostante è stata chiusa: si è verificato un errore imprevisto su un invio*.</span><span class="sxs-lookup"><span data-stu-id="4de38-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>



