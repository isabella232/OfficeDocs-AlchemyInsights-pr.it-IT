---
title: Uno dei certificati del servizio federativo locale è in scadenza
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: 00cbc77cb178d59a3115e44874a16f506e4408c6
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36543569"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a><span data-ttu-id="c986f-102">Uno dei certificati del servizio federativo locale è in scadenza</span><span class="sxs-lookup"><span data-stu-id="c986f-102">One of your on-premises Federation Service Certificates is expiring</span></span>

<span data-ttu-id="c986f-103">Per risolvere il problema, attenersi alla seguente procedura:</span><span class="sxs-lookup"><span data-stu-id="c986f-103">To resolve this issue, follow these steps:</span></span>
  
- <span data-ttu-id="c986f-104">Installare il modulo di Microsoft Azure Active Directory per Windows PowerShell nel computer (se il modulo non è già installato).</span><span class="sxs-lookup"><span data-stu-id="c986f-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="c986f-105">A tale scopo, accedere a [PowerShell di Azure Active Directory per il grafico](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="c986f-105">To do this, go to [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span></span>
    
- <span data-ttu-id="c986f-106">Seguire la procedura descritta nella sezione "scenario 1: il certificato per la firma di token AD FS scaduto" di ["si è verificato un problema durante l'accesso al sito" da ADFS quando un utente federato accede a Office 365, Azure o Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="c986f-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
- <span data-ttu-id="c986f-107">Seguire i passaggi descritti in t[come aggiornare o ripristinare le impostazioni di un dominio federato in Office 365, Azure o Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span><span class="sxs-lookup"><span data-stu-id="c986f-107">Follow the steps in t[How to update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
<span data-ttu-id="c986f-108">Per ulteriori informazioni sul rinnovo dei certificati di federazione, vedere [rinnovo del certificato per O365 e Azure ad](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="c986f-108">For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
  

