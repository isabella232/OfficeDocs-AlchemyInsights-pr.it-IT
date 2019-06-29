---
title: Risoluzione dei problemi relativi alla sincronizzazione delle password
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 165e0ff4b2136b727450946d2c47756ebee7d393
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/28/2019
ms.locfileid: "35353109"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="77be2-102">Risoluzione dei problemi relativi alla sincronizzazione delle password</span><span class="sxs-lookup"><span data-stu-id="77be2-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="77be2-103">Per risolvere i problemi in cui nessuna password è sincronizzata con Azure AD Connect Version 1.1.614.0 o versione successiva:</span><span class="sxs-lookup"><span data-stu-id="77be2-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="77be2-104">Aprire una nuova sessione di Windows PowerShell nel server Azure AD Connect con l'opzione **Esegui come amministratore** .</span><span class="sxs-lookup"><span data-stu-id="77be2-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="77be2-105">Eseguire **Set-ExecutionPolicy RemoteSigned** o **Set-ExecutionPolicy**Unrestricted.</span><span class="sxs-lookup"><span data-stu-id="77be2-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span>

3. <span data-ttu-id="77be2-106">Avviare la procedura guidata di Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="77be2-106">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="77be2-107">Passare alla pagina **attività aggiuntive** , selezionare **risoluzione dei problemi**e quindi fare clic su **Avanti**.</span><span class="sxs-lookup"><span data-stu-id="77be2-107">Navigate to the **Additional Tasks** page, select **Troubleshoot**, and click **Next**.</span></span>

5. <span data-ttu-id="77be2-108">Nella pagina risoluzione dei problemi fare clic su **Avvia per avviare il menu Risoluzione dei problemi** in PowerShell.</span><span class="sxs-lookup"><span data-stu-id="77be2-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span>

6. <span data-ttu-id="77be2-109">Nel menu principale, selezionare **risoluzione dei problemi relativi alla sincronizzazione delle password**.</span><span class="sxs-lookup"><span data-stu-id="77be2-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span>

7. <span data-ttu-id="77be2-110">Nel menu secondario selezionare **sincronizzazione password non funziona affatto**.</span><span class="sxs-lookup"><span data-stu-id="77be2-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span>

<span data-ttu-id="77be2-111">**Informazioni sui risultati dell'attività di risoluzione dei problemi**</span><span class="sxs-lookup"><span data-stu-id="77be2-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="77be2-112">L'attività di risoluzione dei problemi esegue i controlli seguenti:</span><span class="sxs-lookup"><span data-stu-id="77be2-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="77be2-113">Verifica che la funzionalità di sincronizzazione delle password sia abilitata per il tenant di Azure AD.</span><span class="sxs-lookup"><span data-stu-id="77be2-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>

- <span data-ttu-id="77be2-114">Verifica che il server Azure AD Connect non sia in modalità di gestione temporanea.</span><span class="sxs-lookup"><span data-stu-id="77be2-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>

- <span data-ttu-id="77be2-115">Per ogni connettore Active Directory locale esistente (che corrisponde a una foresta di Active Directory esistente):</span><span class="sxs-lookup"><span data-stu-id="77be2-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>

- 
  - <span data-ttu-id="77be2-116">Verifica che la funzionalità di sincronizzazione delle password sia abilitata.</span><span class="sxs-lookup"><span data-stu-id="77be2-116">Validates that the password synchronization feature is enabled.</span></span>

  - <span data-ttu-id="77be2-117">Cerca gli eventi heartbeat di sincronizzazione delle password nei registri eventi applicazioni di Windows.</span><span class="sxs-lookup"><span data-stu-id="77be2-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>

  - <span data-ttu-id="77be2-118">Per ogni dominio di Active Directory sotto il connettore Active Directory locale:</span><span class="sxs-lookup"><span data-stu-id="77be2-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>

  - <span data-ttu-id="77be2-119">Verifica che il dominio sia raggiungibile dal server Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="77be2-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>

  - <span data-ttu-id="77be2-120">Verifica che gli account di servizi di dominio Active Directory utilizzati dal connettore Active Directory locale dispongano del nome utente, della password e delle autorizzazioni corretti necessari per la sincronizzazione delle password.</span><span class="sxs-lookup"><span data-stu-id="77be2-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>

<span data-ttu-id="77be2-121">Per ulteriori informazioni sulla risoluzione dei problemi relativi alla sincronizzazione delle password, vedere [risolvere i problemi di sincronizzazione delle password con Azure ad Connect Sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span><span class="sxs-lookup"><span data-stu-id="77be2-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  