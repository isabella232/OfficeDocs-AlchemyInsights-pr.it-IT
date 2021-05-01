---
title: Problemi con SharePoint sulle macchine Windows 7
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9006484"
- "11070"
ms.openlocfilehash: 787f0e713cc95b590bc494868d5098a25131ac56
ms.sourcegitcommit: d33ab8c73d8af51da782094fb8f8abf7626f4df3
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/28/2021
ms.locfileid: "52066999"
---
# <a name="issues-with-sharepoint-on-windows-7-machines"></a><span data-ttu-id="98fbb-102">Problemi con SharePoint sulle macchine Windows 7</span><span class="sxs-lookup"><span data-stu-id="98fbb-102">Issues with SharePoint on Windows 7 machines</span></span>

<span data-ttu-id="98fbb-103">Se riscontri errori sui computer Windows 7 mentre lavori con SharePoint o OneDrive, potrebbe essere correlato alla deprecazione di TLS 1.0/1.1.</span><span class="sxs-lookup"><span data-stu-id="98fbb-103">If you receive errors on Windows 7 machines while working on SharePoint or OneDrive, they might be related to the deprecation of TLS 1.0/1.1.</span></span> <span data-ttu-id="98fbb-104">Per altre informazioni, vedere:</span><span class="sxs-lookup"><span data-stu-id="98fbb-104">For more information, see:</span></span>

- [<span data-ttu-id="98fbb-105">Preparazione per TLS 1.2 in Office 365 e Office 365 GCC</span><span class="sxs-lookup"><span data-stu-id="98fbb-105">Preparing for TLS 1.2 in Office 365 and Office 365 GCC</span></span>](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- <span data-ttu-id="98fbb-106">TLS1.2 deve essere abilitato nei client Windows 7 SP1/Windows 8.</span><span class="sxs-lookup"><span data-stu-id="98fbb-106">Windows 7 SP1/Windows 8 clients must have TLS1.2 enabled.</span></span> <span data-ttu-id="98fbb-107">Per altre informazioni, vedi [Si verificano  errori di autenticazione quando il client non supporta TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)</span><span class="sxs-lookup"><span data-stu-id="98fbb-107">For more information, see [Authentication errors occur when client doesn't have TLS 1.2 support](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)</span></span>

- <span data-ttu-id="98fbb-108">Installa KB3140245 e crea il valore di registro.</span><span class="sxs-lookup"><span data-stu-id="98fbb-108">Install KB3140245 and create the registry value.</span></span> <span data-ttu-id="98fbb-109">Per altre informazioni, vedi  [Aggiornamento per abilitare TLS 1.1 e TLS 1.2 come protocolli sicuri di WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)</span><span class="sxs-lookup"><span data-stu-id="98fbb-109">For more information, see [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)</span></span>

- <span data-ttu-id="98fbb-110">Per i client Windows 7 SP1/Windows 8, bisogna assicurare che le suite di crittografia siano iinstallate. </span><span class="sxs-lookup"><span data-stu-id="98fbb-110">Windows 7 SP1/Windows 8 clients must ensure latest TLS cipher suites are installed.</span></span> <span data-ttu-id="98fbb-111">Per altre informazioni, vedi [Microsoft Security Advisory 3042058](https://docs.microsoft.com/security-updates/SecurityAdvisories/2015/3042058).</span><span class="sxs-lookup"><span data-stu-id="98fbb-111">For more information, see [Microsoft Security Advisory 3042058](https://docs.microsoft.com/security-updates/SecurityAdvisories/2015/3042058).</span></span> 


