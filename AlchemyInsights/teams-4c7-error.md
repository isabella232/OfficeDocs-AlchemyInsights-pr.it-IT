---
title: Errore di Teams 4c7
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
- "3472"
- "9001211"
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786673"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="a210c-102">Errore 4c7 in Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="a210c-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="a210c-103">Questo errore si verifica perché Microsoft Teams richiede l'autenticazione Forms.</span><span class="sxs-lookup"><span data-stu-id="a210c-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="a210c-104">Quando si distribuisce Active Directory Federation Services (ADFS), l'autenticazione Forms non è abilitata per la rete Intranet per impostazione predefinita.</span><span class="sxs-lookup"><span data-stu-id="a210c-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="a210c-105">Se l'autenticazione integrata di Windows non riesce, viene richiesto di accedere utilizzando l'autenticazione Forms.</span><span class="sxs-lookup"><span data-stu-id="a210c-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="a210c-106">Per risolvere questo problema, abilitare l'autenticazione Forms utilizzando lo snap-in AD FS Microsoft Management Console (MMC) nel computer che dispone della copia locale di Active Directory.</span><span class="sxs-lookup"><span data-stu-id="a210c-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="a210c-107">A tal fine, attenersi alla seguente procedura:</span><span class="sxs-lookup"><span data-stu-id="a210c-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="a210c-108">Nel riquadro di spostamento passare a **Criteri di autenticazione.**</span><span class="sxs-lookup"><span data-stu-id="a210c-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="a210c-109">In **Azioni** nel riquadro dei dettagli selezionare **Modifica autenticazione principale globale**.</span><span class="sxs-lookup"><span data-stu-id="a210c-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="a210c-110">Nella scheda **Intranet** selezionare **Autenticazione Forms**.</span><span class="sxs-lookup"><span data-stu-id="a210c-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="a210c-111">Selezionare **OK** (o **Applica**).</span><span class="sxs-lookup"><span data-stu-id="a210c-111">Select **OK** (or **Apply**).</span></span>