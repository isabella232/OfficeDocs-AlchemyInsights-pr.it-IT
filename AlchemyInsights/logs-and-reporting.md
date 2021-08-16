---
title: Log e report
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004331"
- "7727"
ms.openlocfilehash: 03d77c17622a1aac5ecb035bb5b73efdbbfe5e6b141e6b266eef8783f612c8b2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54067016"
---
# <a name="logs-and-reporting"></a>Log e report

[Azure Active Directory domande frequenti sui report risponde](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) alle domande frequenti sulla creazione di report Azure Active Directory (Azure AD). Per ulteriori informazioni, vedere [Azure Active Directory reporting](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports).

**Risoluzione dei problemi relativi al controllo**

1. Se si verificano problemi durante la visualizzazione di alcune attività di controllo e l'attività mancante è in questo [elenco,](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities)determinare un ticket di supporto.
2. Se si verificano problemi durante la visualizzazione dei log di controllo nel tenant, è necessario determinare un ticket di supporto.
3. Se le attività di controllo non vengono visualizzate immediatamente nel portale di Azure, consultare le informazioni sulla [latenza](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) e archiviare un ticket di supporto se il ritardo supera la latenza documentata.
4. [Conservazione dei log attività di Azure AD](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-data-retention)
5. Se non viene visualizzato tutto il controllo per l'intervallo di date selezionato, è possibile scaricare fino a 250.000 righe (ordinate in base alla più recente) di accesso dal portale di Azure. Per ulteriori informazioni, vedere [Download delle attività di controllo](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report).

**Risoluzione dei problemi relativi agli accesso**

1. È possibile visualizzare gli ultimi 30 giorni di dati solo se si dispone di una licenza Azure AD Premium (P1 o P2) per il tenant.
2. Gli accesso sono disponibili solo per Azure AD Premium tenant. Non è disponibile per i tenant con licenza Free o Basic.
3. Se il tenant ha una licenza Premium P1 e non è possibile visualizzare gli account di accesso, consultare le informazioni sulla [latenza](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) e archiviare un ticket di supporto se il ritardo supera la latenza documentata.
4. Se non vengono visualizzati tutti gli account di accesso per l'intervallo di date selezionato, è possibile scaricare fino a 250.000 righe (ordinate in base alla versione più recente) di accesso dal portale di Azure. Per ulteriori informazioni, vedere [Download delle attività di accesso](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities).

**Risolvere i problemi relativi ai report di sicurezza (utenti contrassegnati a rischio, accesso rischioso)**

1. [Utenti contrassegnati per il report di sicurezza dei rischi](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-user-at-risk)
2. [Report di accesso rischioso nel portale Azure Active Directory utenti](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risky-sign-ins)
3. [Azure Active Directory di rischio](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risk-events)
