---
title: Active Directory non sincronizzato
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
- "9001688"
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: 0da512379e5a2f6ccb773e18c465e545c0660560
ms.sourcegitcommit: e42bb24c9bae1d0df8c49c424d2aa5e7466703ac
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/14/2021
ms.locfileid: "52930979"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="0ad76-102">Active Directory non sincronizzato</span><span class="sxs-lookup"><span data-stu-id="0ad76-102">Active Directory not syncing</span></span>

<span data-ttu-id="0ad76-103">Se si ricevono errori di sincronizzazione, ad esempio "nessuna sincronizzazione recente" o si nota lo stato di sincronizzazione della directory nel portale di amministrazione di Office, "Ultima sincronizzazione più di 3 giorni fa", è possibile che AADConnect abbia impostazioni errate o autorizzazioni insufficienti per eseguire una sincronizzazione.</span><span class="sxs-lookup"><span data-stu-id="0ad76-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="0ad76-104">La reinstallazione di AADConnect tramite impostazioni rapide potrebbe risolvere rapidamente il problema:</span><span class="sxs-lookup"><span data-stu-id="0ad76-104">Reinstalling AADConnect by using express settings might resolve the issue quickly:</span></span>

1. <span data-ttu-id="0ad76-105">[Scaricare la versione più recente di AADConnect.](https://go.microsoft.com/fwlink/?LinkId=615771)</span><span class="sxs-lookup"><span data-stu-id="0ad76-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="0ad76-106">[Seguire le istruzioni per l'installazione rapida](/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="0ad76-106">[Follow the instructions for express installation](/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="0ad76-107">Azure AD Connect deve essere installato in Windows Server 2012 o versione successiva.</span><span class="sxs-lookup"><span data-stu-id="0ad76-107">Azure AD Connect must be installed on Windows Server 2012 or later.</span></span> <span data-ttu-id="0ad76-108">Il server deve essere aggiunto al dominio e può essere un controller di dominio o un server membro.</span><span class="sxs-lookup"><span data-stu-id="0ad76-108">This server must be domain joined and may be a domain controller or a member server.</span></span> <span data-ttu-id="0ad76-109">Per un elenco completo dei requisiti Connessione azure AD e dei prerequisiti, vedere [Prerequisiti per Azure AD Connessione](/azure/active-directory/hybrid/how-to-connect-install-prerequisites).</span><span class="sxs-lookup"><span data-stu-id="0ad76-109">For a full list of Azure AD Connect requirements and pre-requisites, review [Prerequisites for Azure AD Connect](/azure/active-directory/hybrid/how-to-connect-install-prerequisites).</span></span>

<span data-ttu-id="0ad76-110">Per altre informazioni sugli account dei servizi di AADConnect, vedere [Azure AD Connect: account e autorizzazioni](/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span><span class="sxs-lookup"><span data-stu-id="0ad76-110">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
