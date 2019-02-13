---
title: Risoluzione dei problemi di sincronizzazione delle password
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: d346cf97fb2fd08a9132904517192d8728ffa941
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29924700"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="f886e-102">Risoluzione dei problemi di sincronizzazione delle password</span><span class="sxs-lookup"><span data-stu-id="f886e-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="f886e-103">Per la risoluzione dei problemi in alcuna password non sono sincronizzati con Azure Active Directory Connect versione 1.1.614.0 o versione successiva:</span><span class="sxs-lookup"><span data-stu-id="f886e-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="f886e-104">Aprire una nuova sessione di Windows PowerShell nel server di Azure Active Directory Connetti con l'opzione **Esegui come amministratore** .</span><span class="sxs-lookup"><span data-stu-id="f886e-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span> 
    
2. <span data-ttu-id="f886e-105">Eseguire **Set-ExecutionPolicy RemoteSigned** o **Set-ExecutionPolicy Unrestricted**.</span><span class="sxs-lookup"><span data-stu-id="f886e-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span> 
    
3. <span data-ttu-id="f886e-106">Avviare la procedura guidata Connetti Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f886e-106">Start the Azure AD Connect wizard.</span></span>
    
4. <span data-ttu-id="f886e-107">Passare al \* \* necessario eseguire altre attività \* \* pagina selezionare \* \* Troubleshoot \* \*, fare clic su **Avanti**.</span><span class="sxs-lookup"><span data-stu-id="f886e-107">Navigate to the \*\* Additional Tasks \*\* page, select \*\* Troubleshoot \*\*, and click **Next**.</span></span> 
    
5. <span data-ttu-id="f886e-108">Nella pagina di risoluzione dei problemi, fare clic sul menu **Avvia per avviare la risoluzione dei problemi** di PowerShell.</span><span class="sxs-lookup"><span data-stu-id="f886e-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span> 
    
6. <span data-ttu-id="f886e-109">Nel menu principale, selezionare **La sincronizzazione delle Password risolvere i problemi**.</span><span class="sxs-lookup"><span data-stu-id="f886e-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span> 
    
7. <span data-ttu-id="f886e-110">Nel menu sub, selezionare **la sincronizzazione delle Password non funziona affatto**.</span><span class="sxs-lookup"><span data-stu-id="f886e-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span> 
    
 <span data-ttu-id="f886e-111">**Acquisire familiarità con i risultati dell'attività di risoluzione dei problemi**</span><span class="sxs-lookup"><span data-stu-id="f886e-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="f886e-112">L'attività di risoluzione dei problemi consente di eseguire le verifiche seguenti:</span><span class="sxs-lookup"><span data-stu-id="f886e-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="f886e-113">Consente di verificare che la funzionalità di sincronizzazione password è abilitata per il tenant di Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f886e-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>
    
- <span data-ttu-id="f886e-114">Convalida che il server di connessione di Azure Active Directory non è in modalità di gestione temporanea.</span><span class="sxs-lookup"><span data-stu-id="f886e-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>
    
- <span data-ttu-id="f886e-115">Per ogni locale Active Directory connettore esistente (che corrisponde a una foresta di Active Directory esistente):</span><span class="sxs-lookup"><span data-stu-id="f886e-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>
    
- 
  - <span data-ttu-id="f886e-116">Consente di verificare che sia abilitata la funzionalità di sincronizzazione delle password.</span><span class="sxs-lookup"><span data-stu-id="f886e-116">Validates that the password synchronization feature is enabled.</span></span>
    
  - <span data-ttu-id="f886e-117">Cerca password sincronizzazione heartbeat eventi nei registri eventi applicazioni di Windows.</span><span class="sxs-lookup"><span data-stu-id="f886e-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>
    
  - <span data-ttu-id="f886e-118">Per ogni dominio di Active Directory con il connettore di Active Directory locale:</span><span class="sxs-lookup"><span data-stu-id="f886e-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>
    
  - <span data-ttu-id="f886e-119">Verifica che il dominio sia raggiungibile dal server di Azure Active Directory Connetti.</span><span class="sxs-lookup"><span data-stu-id="f886e-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>
    
  - <span data-ttu-id="f886e-120">Consente di verificare che gli account di servizi di dominio Active Directory (AD DS) utilizzati dal connettore di Active Directory locale con la corretta username, password e le autorizzazioni necessarie per la sincronizzazione delle password.</span><span class="sxs-lookup"><span data-stu-id="f886e-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>
    
<span data-ttu-id="f886e-121">Per ulteriore assistenza nella risoluzione dei problemi di sincronizzazione delle password, vedere [Troubleshoot la sincronizzazione delle password con sincronizzazione di Azure Active Directory Connetti](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span><span class="sxs-lookup"><span data-stu-id="f886e-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  

