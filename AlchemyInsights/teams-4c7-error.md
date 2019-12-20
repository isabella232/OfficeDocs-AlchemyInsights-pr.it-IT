---
title: Errore 4C7 Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 0945a341c6456ee4178c0485f3bfb9232fa78a11
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796200"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="f0e1d-102">errore 4C7 in Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="f0e1d-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="f0e1d-103">Questo errore si verifica perché Microsoft teams richiede l'autenticazione basata su form.</span><span class="sxs-lookup"><span data-stu-id="f0e1d-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="f0e1d-104">Quando si distribuisce Active Directory Federation Services (AD FS), l'autenticazione basata su form non è abilitata per impostazione predefinita per la rete Intranet.</span><span class="sxs-lookup"><span data-stu-id="f0e1d-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="f0e1d-105">Se l'autenticazione integrata di Windows ha esito negativo, viene richiesto di eseguire l'accesso utilizzando l'autenticazione basata su form.</span><span class="sxs-lookup"><span data-stu-id="f0e1d-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="f0e1d-106">Per risolvere il problema, abilitare l'autenticazione basata su form mediante lo snap-in di Microsoft Management Console (MMC) di ADFS nel computer in cui è presente la copia locale di Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f0e1d-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="f0e1d-107">A tale scopo, attieniti alla seguente procedura:</span><span class="sxs-lookup"><span data-stu-id="f0e1d-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="f0e1d-108">Nel riquadro di spostamento, passare a **criteri di autenticazione**.</span><span class="sxs-lookup"><span data-stu-id="f0e1d-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="f0e1d-109">In **azioni** nel riquadro dei dettagli, selezionare **Modifica autenticazione primaria globale**.</span><span class="sxs-lookup"><span data-stu-id="f0e1d-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="f0e1d-110">Nella scheda **Intranet** selezionare **autenticazione Forms**.</span><span class="sxs-lookup"><span data-stu-id="f0e1d-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="f0e1d-111">Fare clic su **OK** (o su **applica**).</span><span class="sxs-lookup"><span data-stu-id="f0e1d-111">Select **OK** (or **Apply**).</span></span>