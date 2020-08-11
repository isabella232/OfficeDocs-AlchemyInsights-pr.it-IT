---
title: Componente aggiuntivo Teams per Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "9003233"
ms.openlocfilehash: 74bd424f71a59b80a91b960b815363668bee7036
ms.sourcegitcommit: 1361b2b37fd0201502a1a3547084961de284a3fc
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/11/2020
ms.locfileid: "46617092"
---
# <a name="teams-add-in-for-mac"></a><span data-ttu-id="914df-102">Componente aggiuntivo Teams per Mac</span><span class="sxs-lookup"><span data-stu-id="914df-102">Teams add-in for Mac</span></span>

<span data-ttu-id="914df-103">Per risolvere i problemi relativi a un componente aggiuntivo mancante di Teams per Mac, segui questa procedura:</span><span class="sxs-lookup"><span data-stu-id="914df-103">To troubleshoot a missing Teams add-in for Mac operating system users, follow these steps:</span></span>

<span data-ttu-id="914df-104">**Passaggio 1:** se hai Exchange ibrido locale (2016 CU3 o versione successiva), usa lo strumento Test-HMA.ps1 per confermare che l'autenticazione moderna ibrida è configurata correttamente.</span><span class="sxs-lookup"><span data-stu-id="914df-104">**Step 1:** If you have Hybrid Exchange On-Premises (2016 CU3 or later required), use the Test-HMA.ps1 tool to confirm that Hybrid Modern Authentication is correctly configured.</span></span> <span data-ttu-id="914df-105">Per altre informazioni, vedere [Validare la configurazione dell'autenticazione moderna ibrida con Outlook per iOS e Android](https://aka.ms/AA980zq).</span><span class="sxs-lookup"><span data-stu-id="914df-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/AA980zq).</span></span>  

<span data-ttu-id="914df-106">**Nota:** utilizzare il formato di indirizzo UPN, ad esempio [username@contoso.com](mailto:username@contoso.com), non dominio\nomeutente.</span><span class="sxs-lookup"><span data-stu-id="914df-106">**Note** Use the UPN address format (for example, [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span></span> <span data-ttu-id="914df-107">Eseguire questa operazione anche per gli utenti con cassette postali di Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="914df-107">Do this even for users with Exchange Online mailboxes.</span></span>

<span data-ttu-id="914df-108">**Passaggio 2:** Chiedere all'utente di andare in **Strumenti** > \*\* Account\*\*... in Outlook per Mac, individuare e selezionare l'account.</span><span class="sxs-lookup"><span data-stu-id="914df-108">**Step 2:** Have the user go to **Tools** > **Accounts**... in Outlook for Mac, and find and select the account.</span></span> <span data-ttu-id="914df-109">Verificare che il nome utente elencato sia in formato UPN, ad esempio [username@contoso.com](mailto:username@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="914df-109">Confirm the username listed is in UPN format (for example, [username@contoso.com](mailto:username@contoso.com)).</span></span>

<span data-ttu-id="914df-110">**Passaggio 3:** Verificare che l'utente abbia una licenza di Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="914df-110">**Step 3:** Confirm the user is a licensed Microsoft Teams user.</span></span> <span data-ttu-id="914df-111">L'utente deve usare l'abbonamento a Office 365 per Mac, prodotto versione 16.24 o successiva.</span><span class="sxs-lookup"><span data-stu-id="914df-111">The user must be using the Office 365 for Mac subscription, product version 16.24 or later.</span></span>