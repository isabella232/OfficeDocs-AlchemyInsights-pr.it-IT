---
title: Posizione dei dati
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: c769c17796d805f88afb4d5b32adb7d4a9bb3ce0
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/21/2020
ms.locfileid: "43655286"
---
# <a name="data-location"></a><span data-ttu-id="921d2-102">Posizione dei dati</span><span class="sxs-lookup"><span data-stu-id="921d2-102">Data location</span></span>

<span data-ttu-id="921d2-103">È possibile visualizzare la posizione del tenant nell'interfaccia di amministrazione o connettersi a Exchange Online tramite PowerShell.</span><span class="sxs-lookup"><span data-stu-id="921d2-103">You can view the location of your tenant in the admin center or by connecting to Exchange Online via PowerShell.</span></span>


<span data-ttu-id="921d2-104">**Interfaccia di amministrazione:**</span><span class="sxs-lookup"><span data-stu-id="921d2-104">**Admin center:**</span></span>
1. <span data-ttu-id="921d2-105">Accedere all'interfaccia di [Amministrazione](https://admin.microsoft.com/Adminportal/Home).</span><span class="sxs-lookup"><span data-stu-id="921d2-105">Log in to the [admin center](https://admin.microsoft.com/Adminportal/Home).</span></span>
2. <span data-ttu-id="921d2-106">Selezionare**il profilo dell'organizzazione** **delle impostazioni** > .</span><span class="sxs-lookup"><span data-stu-id="921d2-106">Select **Settings** > **Organization profile**.</span></span>
3. <span data-ttu-id="921d2-107">In **percorso dati**selezionare **Visualizza dettagli**.</span><span class="sxs-lookup"><span data-stu-id="921d2-107">Under **Data location**, select **View details**.</span></span>


<span data-ttu-id="921d2-108">**PowerShell**</span><span class="sxs-lookup"><span data-stu-id="921d2-108">**PowerShell:**</span></span>
1. <span data-ttu-id="921d2-109">Connettersi a Exchange Online tramite Windows PowerShell.</span><span class="sxs-lookup"><span data-stu-id="921d2-109">Connect to Exchange Online by using Windows PowerShell.</span></span>
2. <span data-ttu-id="921d2-110">Eseguire il cmdlet [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) per visualizzare un elenco delle proprietà del tenant.</span><span class="sxs-lookup"><span data-stu-id="921d2-110">Execute the [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet to display a list of your tenant's properties.</span></span> 
3. <span data-ttu-id="921d2-111">Esaminare la proprietà IDOrganizzazione.</span><span class="sxs-lookup"><span data-stu-id="921d2-111">Look at the OrganizationId property.</span></span>

<span data-ttu-id="921d2-112">Quando si dispone del percorso dati per EXO e SPO, è possibile determinare il percorso dei dati per gli altri servizi da [cui si trovano i dati](https://products.office.com/where-is-your-data-located).</span><span class="sxs-lookup"><span data-stu-id="921d2-112">When you have the data location for EXO and SPO, you can determine the data location for other services you may use from [Where your data is located](https://products.office.com/where-is-your-data-located).</span></span>