---
title: OneDrive for Business Web OneDrive reindirizza a Delve
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: 96f23585f7cbce672842f6330ba79816f24dbc41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51799993"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a><span data-ttu-id="2f402-102">Reindirizzato a Delve dopo aver fatto clic su OneDrive</span><span class="sxs-lookup"><span data-stu-id="2f402-102">Redirected to Delve after you click OneDrive</span></span>

<span data-ttu-id="2f402-103">Vedi la nostra guida dettagliata [alla risoluzione dei problemi.](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning)</span><span class="sxs-lookup"><span data-stu-id="2f402-103">See our detailed [Troubleshooting Guide](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span></span>

<span data-ttu-id="2f402-104">Per risolvere il problema, l'amministratore deve concedere agli utenti il diritto di creare il sito siti personali.</span><span class="sxs-lookup"><span data-stu-id="2f402-104">To resolve this problem, the administrator must grant users the right to create their My Sites site.</span></span> <span data-ttu-id="2f402-105">Ciò è dovuto al fatto che la pagina di OneDrive for Business viene creata nei siti personali.</span><span class="sxs-lookup"><span data-stu-id="2f402-105">This is because the OneDrive for Business page is created on My Sites.</span></span>

<span data-ttu-id="2f402-106">Per concedere questo diritto, attenersi alla seguente procedura:</span><span class="sxs-lookup"><span data-stu-id="2f402-106">To grant this right, follow these steps:</span></span>

1. <span data-ttu-id="2f402-107">Nell'interfaccia di amministrazione di SharePoint fare clic **su profili utente.**</span><span class="sxs-lookup"><span data-stu-id="2f402-107">In the SharePoint admin center,click **user profiles**.</span></span>

2. <span data-ttu-id="2f402-108">Nella sezione **Utenti** fare clic **su Gestisci autorizzazioni utente.**</span><span class="sxs-lookup"><span data-stu-id="2f402-108">In the **People** section, click **Manage User Permissions**.</span></span>

3. <span data-ttu-id="2f402-109">Aggiungere gli utenti che richiedono autorizzazioni per creare il sito siti personali.</span><span class="sxs-lookup"><span data-stu-id="2f402-109">Add users who require permissions to create their My Sites site.</span></span> <span data-ttu-id="2f402-110">Per impostazione predefinita, questa impostazione è impostata su **Tutti tranne gli utenti esterni.**</span><span class="sxs-lookup"><span data-stu-id="2f402-110">By default, this setting is set to **Everyone except external users**.</span></span>

4. <span data-ttu-id="2f402-111">Dopo aver aggiunto l'utente, gli utenti o il gruppo, assicurarsi che l'utente, gli utenti o il gruppo aggiunto sia selezionato, scorrere fino alla sezione autorizzazioni e quindi selezionare la casella di controllo accanto a Crea sito personale (necessario per l'archiviazione  **personale, il newsfeed** e il contenuto seguito) .</span><span class="sxs-lookup"><span data-stu-id="2f402-111">After you have added the user, users, or group, make sure that the added user, users, or group is selected, scroll to the **permissions** section, and then select the check box next to **Create Personal Site (required for personal storage, newsfeed, and followed content)**.</span></span>

5. <span data-ttu-id="2f402-112">Fare **clic su OK** e quindi fare in modo che l'utente navigare alla pagina di OneDrive per creare il sito.</span><span class="sxs-lookup"><span data-stu-id="2f402-112">Click **OK**, and then have the user browse to the OneDrive page to create the site.</span></span>
