---
title: Notifica AAD Connect
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
- "9003245"
- "9326"
ms.openlocfilehash: 832c9dd587cb023b5b1d87e905acb123df34237f
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/19/2021
ms.locfileid: "50898044"
---
# <a name="notification-aad-connect"></a><span data-ttu-id="b3e9f-102">Notifica AAD Connect</span><span class="sxs-lookup"><span data-stu-id="b3e9f-102">Notification AAD Connect</span></span>

- <span data-ttu-id="b3e9f-103">Assicurarsi di essere autorizzati a eseguire l'operazione.</span><span class="sxs-lookup"><span data-stu-id="b3e9f-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="b3e9f-104">Gli amministratori globali hanno accesso per impostazione predefinita.</span><span class="sxs-lookup"><span data-stu-id="b3e9f-104">Global Admins have access by default.</span></span> <span data-ttu-id="b3e9f-105">È inoltre possibile utilizzare il controllo di accesso basato sui [ruoli](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) per delegare l'autorizzazione di registrazione a Collaboratore.</span><span class="sxs-lookup"><span data-stu-id="b3e9f-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="b3e9f-106">Verificare che gli endpoint necessari siano abilitati e non bloccati a causa del firewall.</span><span class="sxs-lookup"><span data-stu-id="b3e9f-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="b3e9f-107">Per informazioni dettagliate, vedere [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span><span class="sxs-lookup"><span data-stu-id="b3e9f-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="b3e9f-108">La registrazione può non riuscire a causa della comunicazione in uscita sottoposta all'ispezione SSL da parte del livello di rete.</span><span class="sxs-lookup"><span data-stu-id="b3e9f-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="b3e9f-109">Assicurati di aver verificato le impostazioni di notifica per Azure AD Connect Health ed esamina l'impostazione.</span><span class="sxs-lookup"><span data-stu-id="b3e9f-109">Make sure you have verified the notification settings for Azure AD Connect Health and review your setting.</span></span> <span data-ttu-id="b3e9f-110">Per informazioni su come configurare le impostazioni di notifica per le notifiche di Azure AD Connect Health, vedere questa [guida.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations)</span><span class="sxs-lookup"><span data-stu-id="b3e9f-110">To understand how to configure the notification settings for Azure AD Connect Health notifications, see this [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations).</span></span>
- <span data-ttu-id="b3e9f-111">Per ulteriori informazioni sul report di sincronizzazione dell'integrità di AAD Connect e su come scaricarlo, vedere Report di sincronizzazione [a livello di oggetto.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)</span><span class="sxs-lookup"><span data-stu-id="b3e9f-111">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="b3e9f-112">Per risolvere i problemi relativi agli avvisi di integrità di AAD Connect, seguire la guida alla risoluzione dei problemi per gli avvisi di aggiornamento dei dati di [AAD Connect Health](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) e per le domande più frequenti, vedere Domande comuni sull'installazione di [AAD Connect Health.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)</span><span class="sxs-lookup"><span data-stu-id="b3e9f-112">To troubleshoot AAD Connect Health Alerts follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
