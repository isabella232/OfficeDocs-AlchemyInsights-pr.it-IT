---
title: OneDrive for Business Web OneDrive reindirizza a approfondire
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: 74151ed149c57ceebc841902796189f6638795a9
ms.sourcegitcommit: c5e800313a6f211386a384716e5fa18e7fcc8c1c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/28/2020
ms.locfileid: "41571214"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a><span data-ttu-id="71999-102">Reindirizzato a approfondire dopo aver fatto clic su OneDrive</span><span class="sxs-lookup"><span data-stu-id="71999-102">Redirected to Delve after you click OneDrive</span></span>

<span data-ttu-id="71999-103">Consultare la [Guida alla risoluzione dei problemi](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning)dettagliata.</span><span class="sxs-lookup"><span data-stu-id="71999-103">See our detailed [Troubleshooting Guide](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span></span>

<span data-ttu-id="71999-104">Per risolvere il problema, l'amministratore di Office 365 deve concedere agli utenti il diritto di creare il sito personale.</span><span class="sxs-lookup"><span data-stu-id="71999-104">To resolve this problem, the Office 365 administrator must grant users the right to create their My Sites site.</span></span> <span data-ttu-id="71999-105">Ciò è dovuto al fatto che la pagina di OneDrive for business viene creata nei siti personali.</span><span class="sxs-lookup"><span data-stu-id="71999-105">This is because the OneDrive for Business page is created on My Sites.</span></span>

<span data-ttu-id="71999-106">Per concedere questo diritto, eseguire la procedura seguente:</span><span class="sxs-lookup"><span data-stu-id="71999-106">To grant this right, follow these steps:</span></span>

1. <span data-ttu-id="71999-107">Nell'interfaccia di amministrazione di SharePoint, fare clic su **profili utente**.</span><span class="sxs-lookup"><span data-stu-id="71999-107">In the SharePoint admin center,click **user profiles**.</span></span>

2. <span data-ttu-id="71999-108">Nella sezione **utenti** fare clic su **Gestisci autorizzazioni utente**.</span><span class="sxs-lookup"><span data-stu-id="71999-108">In the **People** section, click **Manage User Permissions**.</span></span>

3. <span data-ttu-id="71999-109">Aggiungere gli utenti che richiedono le autorizzazioni per creare il sito di siti personali.</span><span class="sxs-lookup"><span data-stu-id="71999-109">Add users who require permissions to create their My Sites site.</span></span> <span data-ttu-id="71999-110">Per impostazione predefinita, questa impostazione è impostata su **tutti tranne gli utenti esterni**.</span><span class="sxs-lookup"><span data-stu-id="71999-110">By default, this setting is set to **Everyone except external users**.</span></span>

4. <span data-ttu-id="71999-111">Dopo aver aggiunto l'utente, gli utenti o il gruppo, assicurarsi che l'utente, gli utenti o il gruppo aggiunto siano selezionati, scorrere fino alla sezione **autorizzazioni** e quindi selezionare la casella di controllo accanto a **Crea sito personale (obbligatorio per l'archiviazione personale, newsfeed e contenuto seguito)**.</span><span class="sxs-lookup"><span data-stu-id="71999-111">After you have added the user, users, or group, make sure that the added user, users, or group is selected, scroll to the **permissions** section, and then select the check box next to **Create Personal Site (required for personal storage, newsfeed, and followed content)**.</span></span>

5. <span data-ttu-id="71999-112">Fare clic su **OK**, quindi passare alla pagina OneDrive per creare il sito.</span><span class="sxs-lookup"><span data-stu-id="71999-112">Click **OK**, and then have the user browse to the OneDrive page to create the site.</span></span>
