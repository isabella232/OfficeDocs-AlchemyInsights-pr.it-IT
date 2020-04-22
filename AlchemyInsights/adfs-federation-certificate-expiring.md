---
title: Scadenza del certificato di federazione ADFS
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 14e7da6220dfa96edca5d9ec5c32e003480a9eaf
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43710411"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="4968f-102">Scadenza del certificato di federazione ADFS</span><span class="sxs-lookup"><span data-stu-id="4968f-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="4968f-103">Per risolvere il problema, attenersi alla seguente procedura:</span><span class="sxs-lookup"><span data-stu-id="4968f-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="4968f-104">Installare il modulo di Microsoft Azure Active Directory per Windows PowerShell nel computer (se il modulo non è già installato).</span><span class="sxs-lookup"><span data-stu-id="4968f-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="4968f-105">A tale scopo, passare a [gestione Azure ad tramite Windows PowerShell](https://aka.ms/aadposh).</span><span class="sxs-lookup"><span data-stu-id="4968f-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="4968f-106">Seguire la procedura descritta nella sezione "scenario 1: il certificato per la firma di token AD FS scaduto" di ["si è verificato un problema durante l'accesso al sito" da ADFS quando un utente federato accede a Microsoft 365, Azure o Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="4968f-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="4968f-107">Attenersi alla procedura descritta in [Update or repair the settings of a federato Domain in Microsoft, Azure o Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span><span class="sxs-lookup"><span data-stu-id="4968f-107">Follow the steps in [Update or repair the settings of a federated domain in Microsoft, Azure, or Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span></span>

    <span data-ttu-id="4968f-108">Per ulteriori informazioni su come rinnovare i certificati di federazione, vedere [renew Federation Certificates for Microsoft 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="4968f-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Microsoft 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
