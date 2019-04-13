---
title: 932 aggiornamento di AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 932
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 8ffa8f64019077034bc4fad61d1d843849c42898
ms.sourcegitcommit: 1a4b8fa9e38a95ca811085af516edb81caf2018c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/13/2019
ms.locfileid: "31858964"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="0fda4-102">Aggiornamento di Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="0fda4-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="0fda4-103">Per impostazione predefinita, l'aggiornamento automatico è abilitato per Azure AD Connect, che consente di verificare che la versione più recente sia in esecuzione.</span><span class="sxs-lookup"><span data-stu-id="0fda4-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="0fda4-104">Per verificare le impostazioni di aggiornamento automatico, utilizzare il cmdlet **Get-ADSyncAutoUpgrade** in Azure ad PowerShell.</span><span class="sxs-lookup"><span data-stu-id="0fda4-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="0fda4-105">Il cmdlet restituirà uno dei seguenti valori:</span><span class="sxs-lookup"><span data-stu-id="0fda4-105">The cmdlet will return one of following values:</span></span> 

- <span data-ttu-id="0fda4-106">**Enabled**: l'aggiornamento automatico è abilitato.</span><span class="sxs-lookup"><span data-stu-id="0fda4-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="0fda4-107">**Disabled**: l'aggiornamento automatico è disabilitato.</span><span class="sxs-lookup"><span data-stu-id="0fda4-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="0fda4-108">**Sospesa**: il sistema non è più idoneo per ricevere gli aggiornamenti automatici.</span><span class="sxs-lookup"><span data-stu-id="0fda4-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="0fda4-109">Non è possibile configurare questo valore. viene impostato dal sistema.</span><span class="sxs-lookup"><span data-stu-id="0fda4-109">You can't configure this value; it's set by the system.</span></span> 

<span data-ttu-id="0fda4-110">Per ulteriori informazioni, vedere [aggiornamento automatico](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="0fda4-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="0fda4-111">Per scaricare la versione più recente di Azure AD Connect, passare [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594)a.</span><span class="sxs-lookup"><span data-stu-id="0fda4-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
