---
title: 126 Errore impossibile trovare una cassetta postale in OWA?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 6bab821aaa3b50c365ef5d25a61bca195c76d7ce
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426666"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a><span data-ttu-id="0a1b1-102">Ottenere un errore di cassetta postale non trovato in Outlook sul Web?</span><span class="sxs-lookup"><span data-stu-id="0a1b1-102">Getting a mailbox not found error in Outlook on the web?</span></span>

<span data-ttu-id="0a1b1-103">Se si utilizza Outlook sul Web e non è possibile trovare una cassetta postale per errore, **l'account** utilizzato per connettersi a Outlook sul Web non dispone di una licenza di Exchange Online e pertanto nessuna cassetta postale è associata all'account.</span><span class="sxs-lookup"><span data-stu-id="0a1b1-103">If you're using Outlook on the web and you get a **Mailbox couldn't be found for** error, the account that you used to connect to Outlook on the web doesn't have an Exchange Online license and therefore, no mailbox is associated with the account.</span></span> <span data-ttu-id="0a1b1-104">L'amministratore può assegnare una licenza al tuo account seguendo questi passaggi:</span><span class="sxs-lookup"><span data-stu-id="0a1b1-104">Your admin can assign a license to your account by following these steps:</span></span>

1. <span data-ttu-id="0a1b1-105">Aprire [l'interfaccia di amministrazione di Microsoft 365](https://portal.office.com/adminportal/home#/homepage) e passare **a** Utenti attivi nella sezione Utenti e selezionare l'utente che sta visualizzato l'errore. </span><span class="sxs-lookup"><span data-stu-id="0a1b1-105">Open the [Microsoft 365 admin center](https://portal.office.com/adminportal/home#/homepage) and go to **Active users** under the **Users** section, and select the user who is seeing the error.</span></span>

2. <span data-ttu-id="0a1b1-106">Nella pagina utente visualizzata passare  alla sezione Licenze e  app, selezionare il valore percorso appropriato e assegnare una licenza contenente Exchange Online (espandere la licenza per visualizzarne i dettagli).</span><span class="sxs-lookup"><span data-stu-id="0a1b1-106">In the user page that opens, go to the **Licenses and Apps** section, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details).</span></span> <span data-ttu-id="0a1b1-107">Al termine, fai clic su **salvare le modifiche**.</span><span class="sxs-lookup"><span data-stu-id="0a1b1-107">When you're finished, click **Save changes**.</span></span>

<span data-ttu-id="0a1b1-108">In alcuni casi, se la licenza è già assegnata a un account utente, la rimozione e la riassegnazione della licenza consentono di risolvere il problema e di eseguirne il provisioning nel sistema:</span><span class="sxs-lookup"><span data-stu-id="0a1b1-108">In some cases, if the license is already assigned to a user account, removing and reassigning the license helps to resolve the issue and get it properly provisioned in the system:</span></span> 

- <span data-ttu-id="0a1b1-109">Verificare se le sottoscrizioni M365 Exchange Online (e altre, se disponibili) sono correnti e non sono scadute di recente.</span><span class="sxs-lookup"><span data-stu-id="0a1b1-109">Check to see if your M365 Exchange Online (and other, if you have any) subscriptions are current and have not recently expired.</span></span>

<span data-ttu-id="0a1b1-110">Dopo aver verificato che l'abbonamento non è scaduto e che all'account utente sia stata assegnata una licenza valida, il provisioning della licenza può richiedere fino a 24 ore, quindi potrebbe essere necessario attendere la risoluzione del problema.</span><span class="sxs-lookup"><span data-stu-id="0a1b1-110">Once you have made sure that your subscription has not expired and a valid license has been assigned to the user account, it can take up to 24 hours for license to get provisioned, so you might have to wait for your issue to resolve.</span></span> <span data-ttu-id="0a1b1-111">Per altre info, vedi [Assegnare e gestire le licenze.](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses)</span><span class="sxs-lookup"><span data-stu-id="0a1b1-111">For more info, see [Assign and manage licenses](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses).</span></span>