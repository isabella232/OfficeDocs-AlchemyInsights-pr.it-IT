---
title: Sincronizzazione UPN disattivata
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 31947d7c491e4116ffdb9baadf286cd4fbb50f2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749518"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="9c7cb-102">Sincronizzazione UPN disattivata</span><span class="sxs-lookup"><span data-stu-id="9c7cb-102">UPN sync disabled</span></span>

<span data-ttu-id="9c7cb-103">Se è stata avviata la sincronizzazione con Azure AD prima del 30 marzo 2016, eseguire il seguente cmdlet di Azure AD PowerShell per abilitare la corrispondenza morbida UPN solo per l'organizzazione:</span><span class="sxs-lookup"><span data-stu-id="9c7cb-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="9c7cb-104">**Set-MsolDirSyncFeature-feature EnableSoftMatchOnUpn-Enable $True**</span><span class="sxs-lookup"><span data-stu-id="9c7cb-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="9c7cb-105">La combinazione di tasti UPN è attivata automaticamente per le organizzazioni che hanno iniziato a eseguire la sincronizzazione con Azure AD o dopo il 30 marzo 2016.</span><span class="sxs-lookup"><span data-stu-id="9c7cb-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="9c7cb-106">Per ulteriori informazioni sull'abilitazione della corrispondenza morbida su UPN e altre funzionalità di sincronizzazione, vedere [Azure ad Connect Sync Service Features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span><span class="sxs-lookup"><span data-stu-id="9c7cb-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

