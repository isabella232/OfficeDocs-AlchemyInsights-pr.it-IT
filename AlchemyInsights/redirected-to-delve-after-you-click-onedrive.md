---
title: OneDrive for Business Web OneDrive reindirizza a approfondire
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
- "1870"
- "900072"
ms.openlocfilehash: faa2cf25270a3b74a12aeb63d23ce98b51e13cb6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47776383"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a><span data-ttu-id="109e6-102">Reindirizzato a approfondire dopo aver fatto clic su OneDrive</span><span class="sxs-lookup"><span data-stu-id="109e6-102">Redirected to Delve after you click OneDrive</span></span>

<span data-ttu-id="109e6-103">Consultare la [Guida alla risoluzione dei problemi](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning)dettagliata.</span><span class="sxs-lookup"><span data-stu-id="109e6-103">See our detailed [Troubleshooting Guide](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span></span>

<span data-ttu-id="109e6-104">Per risolvere il problema, l'amministratore deve concedere agli utenti il diritto di creare il sito di siti personali.</span><span class="sxs-lookup"><span data-stu-id="109e6-104">To resolve this problem, the administrator must grant users the right to create their My Sites site.</span></span> <span data-ttu-id="109e6-105">Ciò è dovuto al fatto che la pagina di OneDrive for business viene creata nei siti personali.</span><span class="sxs-lookup"><span data-stu-id="109e6-105">This is because the OneDrive for Business page is created on My Sites.</span></span>

<span data-ttu-id="109e6-106">Per concedere questo diritto, eseguire la procedura seguente:</span><span class="sxs-lookup"><span data-stu-id="109e6-106">To grant this right, follow these steps:</span></span>

1. <span data-ttu-id="109e6-107">Nell'interfaccia di amministrazione di SharePoint, fare clic su **profili utente**.</span><span class="sxs-lookup"><span data-stu-id="109e6-107">In the SharePoint admin center,click **user profiles**.</span></span>

2. <span data-ttu-id="109e6-108">Nella sezione **utenti** fare clic su **Gestisci autorizzazioni utente**.</span><span class="sxs-lookup"><span data-stu-id="109e6-108">In the **People** section, click **Manage User Permissions**.</span></span>

3. <span data-ttu-id="109e6-109">Aggiungere gli utenti che richiedono le autorizzazioni per creare il sito di siti personali.</span><span class="sxs-lookup"><span data-stu-id="109e6-109">Add users who require permissions to create their My Sites site.</span></span> <span data-ttu-id="109e6-110">Per impostazione predefinita, questa impostazione è impostata su **tutti tranne gli utenti esterni**.</span><span class="sxs-lookup"><span data-stu-id="109e6-110">By default, this setting is set to **Everyone except external users**.</span></span>

4. <span data-ttu-id="109e6-111">Dopo aver aggiunto l'utente, gli utenti o il gruppo, assicurarsi che l'utente, gli utenti o il gruppo aggiunto siano selezionati, scorrere fino alla sezione **autorizzazioni** e quindi selezionare la casella di controllo accanto a **Crea sito personale (obbligatorio per l'archiviazione personale, newsfeed e contenuto seguito)**.</span><span class="sxs-lookup"><span data-stu-id="109e6-111">After you have added the user, users, or group, make sure that the added user, users, or group is selected, scroll to the **permissions** section, and then select the check box next to **Create Personal Site (required for personal storage, newsfeed, and followed content)**.</span></span>

5. <span data-ttu-id="109e6-112">Fare clic su **OK**, quindi passare alla pagina OneDrive per creare il sito.</span><span class="sxs-lookup"><span data-stu-id="109e6-112">Click **OK**, and then have the user browse to the OneDrive page to create the site.</span></span>
