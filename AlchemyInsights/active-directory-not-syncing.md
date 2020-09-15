---
title: Active Directory non sincronizzato
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
- "9001688"
- "3754"
ms.openlocfilehash: 3517f424b4dcd89f915acebab747a9bff993fdbd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47697633"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="910d3-102">Active Directory non sincronizzato</span><span class="sxs-lookup"><span data-stu-id="910d3-102">Active Directory not syncing</span></span>

<span data-ttu-id="910d3-103">Se si ricevono errori di sincronizzazione, ad esempio "Nessuna sincronizzazione recente" o si noterà che lo stato di sincronizzazione della directory nel portale di amministrazione di Office dice: "ultima sincronizzazione più di 3 giorni fa", potrebbe essere che AADConnect disponga di impostazioni errate o di autorizzazioni insufficienti per eseguire una sincronizzazione.</span><span class="sxs-lookup"><span data-stu-id="910d3-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="910d3-104">La reinstallazione di AADConnect tramite le impostazioni di Express può risolvere il problema rapidamente:</span><span class="sxs-lookup"><span data-stu-id="910d3-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="910d3-105">[Scaricare la versione più recente di AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span><span class="sxs-lookup"><span data-stu-id="910d3-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="910d3-106">[Seguire le istruzioni per l'installazione espressa](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="910d3-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="910d3-107">Per altre informazioni sugli account dei servizi di AADConnect, vedere [Azure AD Connect: account e autorizzazioni](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span><span class="sxs-lookup"><span data-stu-id="910d3-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
