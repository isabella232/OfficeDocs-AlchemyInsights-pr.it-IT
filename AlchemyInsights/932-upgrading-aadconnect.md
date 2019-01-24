---
title: 932 AADConnect l'aggiornamento
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 9add88a0e4a2590639cbfc546afdcdf5e6aa4886
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/24/2019
ms.locfileid: "29476104"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="436f6-102">Connettere l'aggiornamento Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="436f6-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="436f6-p101">Per impostazione predefinita, l'aggiornamento automatico è abilitata per Azure Active Directory Connect, che consente di verificare che è in esecuzione la versione più recente. Per verificare le impostazioni di aggiornamento automatiche, utilizzare il cmdlet **Get-ADSyncAutoUpgrade** in PowerShell di Azure Active Directory. Il cmdlet restituisce uno dei valori seguenti:</span><span class="sxs-lookup"><span data-stu-id="436f6-p101">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version. To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell. The cmdlet will return one of following values:</span></span> 
  
- <span data-ttu-id="436f6-106">**Enabled**: l'aggiornamento automatico è attivato.</span><span class="sxs-lookup"><span data-stu-id="436f6-106">**Enabled**: Automatic upgrade is enabled.</span></span> 
    
- <span data-ttu-id="436f6-107">**Disabilitata**: l'aggiornamento automatico è disattivato.</span><span class="sxs-lookup"><span data-stu-id="436f6-107">**Disabled**: Automatic upgrade is disabled.</span></span> 
    
- <span data-ttu-id="436f6-p102">**Suspended**: il sistema non è più idoneo ricevere aggiornamenti automatici. Non è possibile configurare questo valore. è impostato dal sistema.</span><span class="sxs-lookup"><span data-stu-id="436f6-p102">**Suspended**: The system is no longer eligible to receive automatic upgrades. You can't configure this value; it's set by the system.</span></span> 
    
<span data-ttu-id="436f6-110">Per ulteriori informazioni, vedere [aggiornamento automatico](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="436f6-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>
  
<span data-ttu-id="436f6-111">Per scaricare la versione più recente di Azure Active Directory Connect, accedere a [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span><span class="sxs-lookup"><span data-stu-id="436f6-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
  

