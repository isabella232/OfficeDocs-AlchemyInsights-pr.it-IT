---
title: Prepararsi per l'uso di TLS 1.2 in Microsoft 365
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Critical
ms.custom:
- "1266"
- "1600052"
ms.assetid: d5c84f5c-a3ca-4abd-8633-7e9ff01328a9
ms.openlocfilehash: 1ec40ba36c69296298e24dca64a873d53682833a
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 11/17/2020
ms.locfileid: "49085908"
---
# <a name="prepare-for-use-of-tls-12-in-microsoft-365"></a><span data-ttu-id="91a52-102">Prepararsi per l'uso di TLS 1.2 in Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="91a52-102">Prepare for use of TLS 1.2 in Microsoft 365</span></span>

<span data-ttu-id="91a52-103">A partire dal 31 ottobre 2018, Microsoft 365 continua il passaggio a TLS 1.2.</span><span class="sxs-lookup"><span data-stu-id="91a52-103">As of October 31st, 2018, Microsoft 365 will continue transitioning to TLS 1.2.</span></span> <span data-ttu-id="91a52-104">A partire dal 15 ottobre 2020, Office 365 inizierà la deprecazione di TLS 1.0 e 1.1 in tutto il servizio.</span><span class="sxs-lookup"><span data-stu-id="91a52-104">Starting October 15, 2020, O365 will begin the deprecation of TLS 1.0 and 1.1 across the service.</span></span> <span data-ttu-id="91a52-105">L'implementazione di questa modifica continuerà nelle prossime settimane e nei prossimi mesi, ma i clienti dovrebbero prendere in considerazione il fatto che le chiamate TLS 1.0/1.1 non funzioneranno con Office 365 a partire dal 15 ott 2020.</span><span class="sxs-lookup"><span data-stu-id="91a52-105">The rollout of this change will continue over the next few weeks and months, but customers should assume no TLS 1.0/1.1 calls will work when engaging with O365 starting Oct 15, 2020.</span></span> <span data-ttu-id="91a52-106">Come già comunicato (MC126199 in Dec 2017, MC128929 in feb 2018, MC186827 nel luglio 2019 e MC218794 nel mese di luglio 2020), stiamo trasferendo tutti i nostri servizi online in Transport Layer Security (TLS) 1.2 + per fornire una crittografia ottimale e per assicurare che il servizio sia più sicuro per impostazione predefinita.</span><span class="sxs-lookup"><span data-stu-id="91a52-106">As previously communicated (MC126199 in Dec 2017, MC128929 in Feb 2018, MC186827 in July 2019, and MC218794 in July 2020), we are moving all of our online services to Transport Layer Security (TLS) 1.2+ to provide best-in-class encryption, and to ensure our service is more secure, by default.</span></span> <span data-ttu-id="91a52-107">I clienti possono comunque scegliere di avere TLS 1.0/1.1 nei propri server e risorse, ma si presume che l'uso di solo TLS 1.2 o versione successiva funzioni quando interagisce con le risorse di Office 365.</span><span class="sxs-lookup"><span data-stu-id="91a52-107">Customers can still choose to have TLS 1.0/1.1 on their servers and resources, but they should assume only TLS 1.2 or higher will work when interacting with O365 resources.</span></span>
  
<span data-ttu-id="91a52-108">Per altre informazioni su queste modifiche, vedere [qui](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide) e [qui](https://docs.microsoft.com/microsoft-365/compliance/tls-1.0-and-1.1-deprecation-for-office-365?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="91a52-108">To learn more about these changes, please see [here](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide) and [here](https://docs.microsoft.com/microsoft-365/compliance/tls-1.0-and-1.1-deprecation-for-office-365?view=o365-worldwide).</span></span>

  