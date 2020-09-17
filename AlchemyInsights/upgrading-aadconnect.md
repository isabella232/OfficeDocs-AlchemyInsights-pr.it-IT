---
title: 932 aggiornamento di AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 5c8ec5d9282c53c655e28f5d38fe36fc3ab005b8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806043"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="956ea-102">Aggiornamento di Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="956ea-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="956ea-103">Per impostazione predefinita, l'aggiornamento automatico è abilitato per Azure AD Connect, che consente di verificare che la versione più recente sia in esecuzione.</span><span class="sxs-lookup"><span data-stu-id="956ea-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="956ea-104">Per verificare le impostazioni di aggiornamento automatico, utilizzare il cmdlet **Get-ADSyncAutoUpgrade** in Azure ad PowerShell.</span><span class="sxs-lookup"><span data-stu-id="956ea-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="956ea-105">Il cmdlet restituirà uno dei seguenti valori:</span><span class="sxs-lookup"><span data-stu-id="956ea-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="956ea-106">**Enabled**: l'aggiornamento automatico è abilitato.</span><span class="sxs-lookup"><span data-stu-id="956ea-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="956ea-107">**Disabled**: l'aggiornamento automatico è disabilitato.</span><span class="sxs-lookup"><span data-stu-id="956ea-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="956ea-108">**Sospesa**: il sistema non è più idoneo per ricevere gli aggiornamenti automatici.</span><span class="sxs-lookup"><span data-stu-id="956ea-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="956ea-109">Non è possibile configurare questo valore. viene impostato dal sistema.</span><span class="sxs-lookup"><span data-stu-id="956ea-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="956ea-110">Per ulteriori informazioni, vedere [aggiornamento automatico](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="956ea-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="956ea-111">Per scaricare la versione più recente di Azure AD Connect, passare a [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .</span><span class="sxs-lookup"><span data-stu-id="956ea-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
