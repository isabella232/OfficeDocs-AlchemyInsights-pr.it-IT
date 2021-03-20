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
# <a name="notification-aad-connect"></a>Notifica AAD Connect

- Assicurarsi di essere autorizzati a eseguire l'operazione. Gli amministratori globali hanno accesso per impostazione predefinita. È inoltre possibile utilizzare il controllo di accesso basato sui [ruoli](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) per delegare l'autorizzazione di registrazione a Collaboratore.
- Verificare che gli endpoint necessari siano abilitati e non bloccati a causa del firewall. Per informazioni dettagliate, vedere [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).
- La registrazione può non riuscire a causa della comunicazione in uscita sottoposta all'ispezione SSL da parte del livello di rete.
- Assicurati di aver verificato le impostazioni di notifica per Azure AD Connect Health ed esamina l'impostazione. Per informazioni su come configurare le impostazioni di notifica per le notifiche di Azure AD Connect Health, vedere questa [guida.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations)
- Per ulteriori informazioni sul report di sincronizzazione dell'integrità di AAD Connect e su come scaricarlo, vedere Report di sincronizzazione [a livello di oggetto.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)

Per risolvere i problemi relativi agli avvisi di integrità di AAD Connect, seguire la guida alla risoluzione dei problemi per gli avvisi di aggiornamento dei dati di [AAD Connect Health](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) e per le domande più frequenti, vedere Domande comuni sull'installazione di [AAD Connect Health.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)
