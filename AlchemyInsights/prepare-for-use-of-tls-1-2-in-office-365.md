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
ms.openlocfilehash: 79a9dc3833f8329adeb24d27014d08c14eb93d1f5f840c5cfa2ce10991107b1c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54040402"
---
# <a name="prepare-for-use-of-tls-12-in-microsoft-365"></a>Prepararsi per l'uso di TLS 1.2 in Microsoft 365

A partire dal 31 ottobre 2018, Microsoft 365 continua il passaggio a TLS 1.2. A partire dal 15 ottobre 2020, Office 365 inizierà la deprecazione di TLS 1.0 e 1.1 in tutto il servizio. L'implementazione di questa modifica continuerà nelle prossime settimane e nei prossimi mesi, ma i clienti dovrebbero prendere in considerazione il fatto che le chiamate TLS 1.0/1.1 non funzioneranno con Office 365 a partire dal 15 ott 2020. Come già comunicato (MC126199 in Dec 2017, MC128929 in feb 2018, MC186827 nel luglio 2019 e MC218794 nel mese di luglio 2020), stiamo trasferendo tutti i nostri servizi online in Transport Layer Security (TLS) 1.2 + per fornire una crittografia ottimale e per assicurare che il servizio sia più sicuro per impostazione predefinita. I clienti possono comunque scegliere di avere TLS 1.0/1.1 nei propri server e risorse, ma si presume che l'uso di solo TLS 1.2 o versione successiva funzioni quando interagisce con le risorse di Office 365.
  
Per altre informazioni su queste modifiche, vedere [qui](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide) e [qui](https://docs.microsoft.com/microsoft-365/compliance/tls-1.0-and-1.1-deprecation-for-office-365?view=o365-worldwide).

  