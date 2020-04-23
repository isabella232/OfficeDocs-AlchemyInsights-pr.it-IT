---
title: 932 aggiornamento di AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: fcc5fddb5cfd15407d0533449035317d187931ed
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766497"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="89a23-102">Aggiornamento di Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="89a23-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="89a23-103">Per impostazione predefinita, l'aggiornamento automatico è abilitato per Azure AD Connect, che consente di verificare che la versione più recente sia in esecuzione.</span><span class="sxs-lookup"><span data-stu-id="89a23-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="89a23-104">Per verificare le impostazioni di aggiornamento automatico, utilizzare il cmdlet **Get-ADSyncAutoUpgrade** in Azure ad PowerShell.</span><span class="sxs-lookup"><span data-stu-id="89a23-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="89a23-105">Il cmdlet restituirà uno dei seguenti valori:</span><span class="sxs-lookup"><span data-stu-id="89a23-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="89a23-106">**Enabled**: l'aggiornamento automatico è abilitato.</span><span class="sxs-lookup"><span data-stu-id="89a23-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="89a23-107">**Disabled**: l'aggiornamento automatico è disabilitato.</span><span class="sxs-lookup"><span data-stu-id="89a23-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="89a23-108">**Sospesa**: il sistema non è più idoneo per ricevere gli aggiornamenti automatici.</span><span class="sxs-lookup"><span data-stu-id="89a23-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="89a23-109">Non è possibile configurare questo valore. viene impostato dal sistema.</span><span class="sxs-lookup"><span data-stu-id="89a23-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="89a23-110">Per ulteriori informazioni, vedere [aggiornamento automatico](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="89a23-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="89a23-111">Per scaricare la versione più recente di Azure AD Connect, passare [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594)a.</span><span class="sxs-lookup"><span data-stu-id="89a23-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
