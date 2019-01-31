---
title: Sincronizzazione UPN disabilitato
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 027782bb2a6b892df6201f3c3bf55151ef7b9db7
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/30/2019
ms.locfileid: "29657975"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="0ca68-102">Sincronizzazione UPN disabilitato</span><span class="sxs-lookup"><span data-stu-id="0ca68-102">UPN sync disabled</span></span>

<span data-ttu-id="0ca68-103">Se è stata avviata la sincronizzazione di Azure Active Directory prima di 30 marzo 2016, eseguire il seguente cmdlet PowerShell di Azure Active Directory per abilitare UPN soft è adatto solo l'organizzazione:</span><span class="sxs-lookup"><span data-stu-id="0ca68-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="0ca68-104">**Set-MsolDirSyncFeature-Feature EnableSoftMatchOnUpn-abilitare $True**</span><span class="sxs-lookup"><span data-stu-id="0ca68-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="0ca68-105">Corrispondenza soft UPN è attivata automaticamente per le organizzazioni che ha avviato la sincronizzazione di Azure Active Directory o dopo 30 marzo 2016.</span><span class="sxs-lookup"><span data-stu-id="0ca68-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="0ca68-106">Per ulteriori informazioni sull'abilitazione di corrispondenza soft UPN e altre funzionalità di sincronizzazione, vedere [caratteristiche del servizio di sincronizzazione Connetti Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span><span class="sxs-lookup"><span data-stu-id="0ca68-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

