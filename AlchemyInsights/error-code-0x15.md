---
title: Codice di errore 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Se si riceve un errore durante l'attivazione di Office 2013 nelle distribuzioni di Servizi Desktop remoto (RDS), è consigliabile abilitare ADAL modificando il registro di sistema.
ms.openlocfilehash: 6d4076ecb5c6ee3c3cf4c4610ad4aa29ab477d8a
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32402743"
---
<span data-ttu-id="e61c3-103">Se si riceve un errore durante l'attivazione di Office 2013 nelle distribuzioni di Servizi Desktop remoto (RDS), è consigliabile abilitare ADAL modificando il registro di sistema.</span><span class="sxs-lookup"><span data-stu-id="e61c3-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span> 
  
|<span data-ttu-id="e61c3-104">**Chiave del Registro di sistema**</span><span class="sxs-lookup"><span data-stu-id="e61c3-104">**Registry key**</span></span>|<span data-ttu-id="e61c3-105">**Tipo**</span><span class="sxs-lookup"><span data-stu-id="e61c3-105">**Type**</span></span>|<span data-ttu-id="e61c3-106">**Valore**</span><span class="sxs-lookup"><span data-stu-id="e61c3-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="e61c3-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="e61c3-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="e61c3-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="e61c3-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="e61c3-109">1 </span><span class="sxs-lookup"><span data-stu-id="e61c3-109">1</span></span>  <br/> |
   
<span data-ttu-id="e61c3-110">Per ulteriori informazioni, vedere [abilitare l'autenticazione moderna per Office 2013 nei dispositivi Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="e61c3-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="e61c3-111">ADAL è abilitato per impostazione predefinita in Office 365 ProPlus e Office 2016.</span><span class="sxs-lookup"><span data-stu-id="e61c3-111">ADAL is enabled by default in Office 365 ProPlus and Office 2016.</span></span> <span data-ttu-id="e61c3-112">i Servizi Desktop remoto (RDS) di > sono stati precedentemente denominati Servizi terminal.</span><span class="sxs-lookup"><span data-stu-id="e61c3-112">>  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span> 
  

