---
title: Codice di errore 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Se si riceve un errore durante l'attivazione di Office 2013 nelle distribuzioni di Servizi Desktop remoto (RDS), è consigliabile abilitare ADAL modificando il registro di sistema.
ms.openlocfilehash: 468d13e59602cf173ed2e17af44c66babfc28703
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506850"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="737e5-103">Errore durante l'attivazione di Office 2013 su Servizi Desktop remoto</span><span class="sxs-lookup"><span data-stu-id="737e5-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="737e5-104">Se si riceve un errore durante l'attivazione di Office 2013 nelle distribuzioni di Servizi Desktop remoto (RDS), è consigliabile abilitare ADAL modificando il registro di sistema.</span><span class="sxs-lookup"><span data-stu-id="737e5-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="737e5-105">**Chiave del Registro di sistema**</span><span class="sxs-lookup"><span data-stu-id="737e5-105">**Registry key**</span></span>|<span data-ttu-id="737e5-106">**Tipo**</span><span class="sxs-lookup"><span data-stu-id="737e5-106">**Type**</span></span>|<span data-ttu-id="737e5-107">**Valore**</span><span class="sxs-lookup"><span data-stu-id="737e5-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="737e5-108">HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="737e5-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="737e5-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="737e5-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="737e5-110">1 </span><span class="sxs-lookup"><span data-stu-id="737e5-110">1</span></span>  <br/> |

<span data-ttu-id="737e5-111">Per ulteriori informazioni, vedere [abilitare l'autenticazione moderna per Office 2013 nei dispositivi Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="737e5-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="737e5-112">ADAL è abilitato per impostazione predefinita in Microsoft 365 Apps for Enterprise e Office 2016.</span><span class="sxs-lookup"><span data-stu-id="737e5-112">ADAL is enabled by default in Microsoft 365 Apps for enterprise and Office 2016.</span></span> <span data-ttu-id="737e5-113">I Servizi Desktop remoto (RDS) sono stati precedentemente denominati Servizi terminal.</span><span class="sxs-lookup"><span data-stu-id="737e5-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  