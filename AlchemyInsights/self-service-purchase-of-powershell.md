---
title: Acquisto in modalità self-service di PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3516"
ms.openlocfilehash: 5e47e08e3309b3d58908e10ee06021da00f230bb
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091721"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="d0af7-102">Acquisto in modalità self-service di PowerShell</span><span class="sxs-lookup"><span data-stu-id="d0af7-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="d0af7-103">Per utilizzare il modulo di MSCommerce PowerShell, è necessario installarlo su un dispositivo Windows 10 con TLS 1,2 (autorizzazioni di amministratore locale necessarie).</span><span class="sxs-lookup"><span data-stu-id="d0af7-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="d0af7-104">Importare e connettersi al modulo MSCommerce.</span><span class="sxs-lookup"><span data-stu-id="d0af7-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="d0af7-105">Quando viene richiesto di eseguire l'accesso, sarà necessario utilizzare le credenziali del ruolo di amministratore globale o di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="d0af7-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="d0af7-106">Se non si dispone di TLS 1,2, è possibile che venga visualizzato il seguente messaggio di errore quando si tenta di ottenere o aggiornare il criterio:</span><span class="sxs-lookup"><span data-stu-id="d0af7-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="d0af7-107">*ErrorMessage-la connessione sottostante è stata chiusa: si è verificato un errore imprevisto su un invio*.</span><span class="sxs-lookup"><span data-stu-id="d0af7-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>



