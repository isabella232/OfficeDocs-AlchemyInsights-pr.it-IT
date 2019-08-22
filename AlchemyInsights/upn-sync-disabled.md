---
title: Sincronizzazione UPN disattivata
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: f390d659b191fa4c44bd7c8acb32409cd3021489
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36532335"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="03ffa-102">Sincronizzazione UPN disattivata</span><span class="sxs-lookup"><span data-stu-id="03ffa-102">UPN sync disabled</span></span>

<span data-ttu-id="03ffa-103">Se è stata avviata la sincronizzazione con Azure AD prima del 30 marzo 2016, eseguire il seguente cmdlet di Azure AD PowerShell per abilitare la corrispondenza morbida UPN solo per l'organizzazione:</span><span class="sxs-lookup"><span data-stu-id="03ffa-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="03ffa-104">**Set-MsolDirSyncFeature-feature EnableSoftMatchOnUpn-Enable $True**</span><span class="sxs-lookup"><span data-stu-id="03ffa-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="03ffa-105">La combinazione di tasti UPN è attivata automaticamente per le organizzazioni che hanno iniziato a eseguire la sincronizzazione con Azure AD o dopo il 30 marzo 2016.</span><span class="sxs-lookup"><span data-stu-id="03ffa-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="03ffa-106">Per ulteriori informazioni sull'abilitazione della corrispondenza morbida su UPN e altre funzionalità di sincronizzazione, vedere [Azure ad Connect Sync Service Features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span><span class="sxs-lookup"><span data-stu-id="03ffa-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

