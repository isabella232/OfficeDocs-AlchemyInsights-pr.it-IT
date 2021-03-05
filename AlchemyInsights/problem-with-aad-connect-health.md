---
title: Problema con AAD Connect Health
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004649"
- "8427"
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/04/2021
ms.locfileid: "50453294"
---
# <a name="problem-with-aad-connect-health"></a><span data-ttu-id="03e6c-102">Problema con AAD Connect Health</span><span class="sxs-lookup"><span data-stu-id="03e6c-102">Problem with AAD Connect Health</span></span>

- <span data-ttu-id="03e6c-103">Assicurarsi di essere autorizzati a eseguire l'operazione.</span><span class="sxs-lookup"><span data-stu-id="03e6c-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="03e6c-104">Gli amministratori globali hanno accesso per impostazione predefinita.</span><span class="sxs-lookup"><span data-stu-id="03e6c-104">Global Admins have access by default.</span></span> <span data-ttu-id="03e6c-105">È inoltre possibile utilizzare il controllo di accesso basato sui [ruoli](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) per delegare l'autorizzazione di registrazione a Collaboratore.</span><span class="sxs-lookup"><span data-stu-id="03e6c-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="03e6c-106">Verificare che gli endpoint necessari siano abilitati e non bloccati a causa del firewall.</span><span class="sxs-lookup"><span data-stu-id="03e6c-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="03e6c-107">Per informazioni dettagliate, vedere [requisiti.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)</span><span class="sxs-lookup"><span data-stu-id="03e6c-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="03e6c-108">La registrazione può non riuscire a causa della comunicazione in uscita sottoposta all'ispezione SSL da parte del livello di rete.</span><span class="sxs-lookup"><span data-stu-id="03e6c-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="03e6c-109">Verificare di aver verificato le impostazioni di notifica per Azure AD Connect Health.</span><span class="sxs-lookup"><span data-stu-id="03e6c-109">Make sure you have verified the notification settings for Azure AD Connect Health.</span></span> <span data-ttu-id="03e6c-110">Controlla le impostazioni.</span><span class="sxs-lookup"><span data-stu-id="03e6c-110">Please review your setting.</span></span> <span data-ttu-id="03e6c-111">Questa [guida](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) può aiutarti a comprendere come configurare le impostazioni di notifica per le notifiche sull'integrità di Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="03e6c-111">This [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) can help you understand how to configure the notification settings for Azure AD Connect health notifications.</span></span>
- <span data-ttu-id="03e6c-112">Per ulteriori informazioni sul report di sincronizzazione dell'integrità di AAD Connect e su come scaricarlo, vedere Report di sincronizzazione [a livello di oggetto.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)</span><span class="sxs-lookup"><span data-stu-id="03e6c-112">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="03e6c-113">Per risolvere i problemi relativi agli avvisi di integrità di AAD Connect, seguire la guida alla risoluzione dei problemi per gli avvisi di aggiornamento dei dati di [AAD Connect Health](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) e per le domande frequenti, vedere domande sull'installazione di [Common AAD Connect Health.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)</span><span class="sxs-lookup"><span data-stu-id="03e6c-113">To troubleshoot AAD Connect Health alerts, follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
