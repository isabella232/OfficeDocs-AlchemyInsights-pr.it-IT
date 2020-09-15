---
title: Risoluzione dei problemi relativi alla sincronizzazione delle password
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 96f63f2ae8e5de246bce7fc15a9b2c3d604f2eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664930"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="82944-102">Risoluzione dei problemi relativi alla sincronizzazione delle password</span><span class="sxs-lookup"><span data-stu-id="82944-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="82944-103">Per risolvere i problemi di sincronizzazione delle password, iniziare a utilizzare questa attività per la risoluzione dei problemi di AAD Connect per determinare il motivo per cui le password non vengono sincronizzate.</span><span class="sxs-lookup"><span data-stu-id="82944-103">To troubleshoot password synchronization issues, start by using this AAD Connect troubleshooting task to determine why passwords are not syncing.</span></span> <span data-ttu-id="82944-104">Per iniziare, passare a [Gestione sincronizzazione diretta](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span><span class="sxs-lookup"><span data-stu-id="82944-104">To begin, go to [Manage direct sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span></span>  

1. <span data-ttu-id="82944-105">Aprire una nuova sessione di Windows PowerShell nel server Azure AD Connect e selezionare l'opzione **Esegui come amministratore** .</span><span class="sxs-lookup"><span data-stu-id="82944-105">Open a new Windows PowerShell session on your Azure AD Connect server, and select the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="82944-106">Eseguire Set-ExecutionPolicy RemoteSigned o Set-ExecutionPolicy Unrestricted.</span><span class="sxs-lookup"><span data-stu-id="82944-106">Run Set-ExecutionPolicy RemoteSigned or Set-ExecutionPolicy Unrestricted.</span></span>

3. <span data-ttu-id="82944-107">Avviare la procedura guidata di Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="82944-107">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="82944-108">Passare alla pagina attività aggiuntive > **risoluzione dei problemi**  >  **successiva**.</span><span class="sxs-lookup"><span data-stu-id="82944-108">Go to the Additional Tasks page > **Troubleshoot** > **Next**.</span></span>

5. <span data-ttu-id="82944-109">Selezionare **Avvia** per aprire il menu di risoluzione dei problemi di PowerShell.</span><span class="sxs-lookup"><span data-stu-id="82944-109">Select **Launch** to open the PowerShell troubleshooting menu.</span></span>

6. <span data-ttu-id="82944-110">Selezionare **risoluzione dei problemi relativi alla sincronizzazione delle password**.</span><span class="sxs-lookup"><span data-stu-id="82944-110">Select **Troubleshoot Password Synchronization**.</span></span>

    <span data-ttu-id="82944-111">Il problema è in genere che non viene sincronizzata una password per un account utente specifico.</span><span class="sxs-lookup"><span data-stu-id="82944-111">The issue is usually that a password is not synchronized for a specific user account.</span></span>

    <span data-ttu-id="82944-112">**Note** La sincronizzazione delle password ha esito negativo se l'ultima sincronizzazione della password è stata completata qualche tempo fa.</span><span class="sxs-lookup"><span data-stu-id="82944-112">**Notes** Password synchronization fails if the last successful password sync was some time ago.</span></span>

<span data-ttu-id="82944-113">Per ulteriori informazioni sulla risoluzione dei problemi relativi alla sincronizzazione delle password, vedere [Troubleshoot password hash Synchronization with Azure ad Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="82944-113">For more help troubleshooting password synchronization, see [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>