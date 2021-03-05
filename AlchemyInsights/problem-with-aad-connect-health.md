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
# <a name="problem-with-aad-connect-health"></a>Problema con AAD Connect Health

- Assicurarsi di essere autorizzati a eseguire l'operazione. Gli amministratori globali hanno accesso per impostazione predefinita. È inoltre possibile utilizzare il controllo di accesso basato sui [ruoli](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) per delegare l'autorizzazione di registrazione a Collaboratore.
- Verificare che gli endpoint necessari siano abilitati e non bloccati a causa del firewall. Per informazioni dettagliate, vedere [requisiti.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)
- La registrazione può non riuscire a causa della comunicazione in uscita sottoposta all'ispezione SSL da parte del livello di rete.
- Verificare di aver verificato le impostazioni di notifica per Azure AD Connect Health. Controlla le impostazioni. Questa [guida](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) può aiutarti a comprendere come configurare le impostazioni di notifica per le notifiche sull'integrità di Azure AD Connect.
- Per ulteriori informazioni sul report di sincronizzazione dell'integrità di AAD Connect e su come scaricarlo, vedere Report di sincronizzazione [a livello di oggetto.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)

Per risolvere i problemi relativi agli avvisi di integrità di AAD Connect, seguire la guida alla risoluzione dei problemi per gli avvisi di aggiornamento dei dati di [AAD Connect Health](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) e per le domande frequenti, vedere domande sull'installazione di [Common AAD Connect Health.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)
