---
title: Eliminare un utente isolato da un server locale
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 537ae7edebfa5a4ab71c2141d549d732ed4f883f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680139"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a><span data-ttu-id="7ca66-102">Eliminare un utente isolato da un server locale</span><span class="sxs-lookup"><span data-stu-id="7ca66-102">Delete orphaned user from on-premises server</span></span>

<span data-ttu-id="7ca66-103">Per rimuovere un utente isolato, procedere come segue:</span><span class="sxs-lookup"><span data-stu-id="7ca66-103">To remove an orphaned user, follow these steps:</span></span>

1. <span data-ttu-id="7ca66-104">Forzare la sincronizzazione della directory seguendo le istruzioni in [Che cos'è l'identità ibrida con Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span><span class="sxs-lookup"><span data-stu-id="7ca66-104">Force directory synchronization by following the instructions in [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span></span>

2. <span data-ttu-id="7ca66-105">Per verificare la sincronizzazione della directory, vedere [Che cos'è l'identità ibrida con Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span><span class="sxs-lookup"><span data-stu-id="7ca66-105">To verify directory synchronization, see [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span></span>

3. <span data-ttu-id="7ca66-106">Se la sincronizzazione funziona correttamente, ma l'eliminazione dell'oggetto di Active Directory non viene propagata in Azure AD, rimuovere manualmente l'oggetto isolato usando uno dei cmdlet seguenti del modulo Azure Active Directory per Windows PowerShell:</span><span class="sxs-lookup"><span data-stu-id="7ca66-106">If sync functions correctly but the Active Directory object deletion does not propagate to Azure AD, manually remove the orphaned object by using one of the following Azure Active Directory Module for Windows PowerShell cmdlets:</span></span>

    <span data-ttu-id="7ca66-107">Remove-MsolContact</span><span class="sxs-lookup"><span data-stu-id="7ca66-107">Remove-MsolContact</span></span>  
    <span data-ttu-id="7ca66-108">Remove-MsolGroup</span><span class="sxs-lookup"><span data-stu-id="7ca66-108">Remove-MsolGroup</span></span>  
    <span data-ttu-id="7ca66-109">Remove-MsolUser</span><span class="sxs-lookup"><span data-stu-id="7ca66-109">Remove-MsolUser</span></span>

    <span data-ttu-id="7ca66-110">Ad esempio, per rimuovere l'ID utente isolato john.smith@contoso.com, creato in origine con la sincronizzazione della directory, eseguire il cmdlet:</span><span class="sxs-lookup"><span data-stu-id="7ca66-110">For example, to remove orphaned user ID john.smith@contoso.com, originally created by using directory synchronization, run the cmdlet:</span></span>

    <span data-ttu-id="7ca66-111">Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com</span><span class="sxs-lookup"><span data-stu-id="7ca66-111">Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com</span></span>