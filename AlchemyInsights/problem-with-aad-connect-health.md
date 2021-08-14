---
title: Problema con AAD Connessione Health
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
ms.openlocfilehash: 82cfcc6132549b52278b174fce3173f5566268864a207882a4dd639cb8024ee3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923756"
---
# <a name="problem-with-aad-connect-health"></a>Problema con AAD Connessione Health

- Assicurarsi di essere autorizzati a eseguire l'operazione. Gli amministratori globali hanno accesso per impostazione predefinita. È inoltre possibile utilizzare il controllo di accesso basato sui [ruoli](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) per delegare l'autorizzazione di registrazione a Collaboratore.
- Verificare che gli endpoint necessari siano abilitati e non bloccati a causa del firewall. Per informazioni dettagliate, vedere [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).
- La registrazione può non riuscire a causa della comunicazione in uscita sottoposta all'ispezione SSL da parte del livello di rete.
- Verificare di aver verificato le impostazioni di notifica per Azure AD Connessione Health. Rivedere l'impostazione. Questa [guida](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) consente di comprendere come configurare le impostazioni di notifica per le notifiche di integrità Connessione Azure AD.
- Per ulteriori informazioni sul report di sincronizzazione dell'integrità Connessione AAD e su come scaricarlo, vedere Report di sincronizzazione [a livello di oggetto.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)

Per risolvere i problemi relativi agli avvisi di integrità di AAD Connessione, seguire la guida alla risoluzione dei problemi per gli avvisi di aggiornamento dei dati di integrità di [AAD Connessione](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) e per le domande frequenti, vedere Domande frequenti sull'installazione di [AAD Connessione Health](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).
