---
title: App di autenticazione
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003252"
- "9909"
ms.openlocfilehash: 1ac3158914455502d2de493dd1320034b1d09573ebb3ffef24c23eb1e816cad0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54082946"
---
# <a name="authentication-app"></a>App di autenticazione

Se sei un amministratore globale, puoi scoprire rapidamente cosa è successo o diagnosticare i problemi relativi all'accesso utente usando [Diagnostica accesso.](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. Avviare la diagnostica facendo clic[sul pulsante](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)" Avvia diagnostica ". 
1. Trova l'evento da analizzare immettendo i dettagli relativi all'utente, all'applicazione, all'ora di accesso, all'ID richiesta o all'ID correlazione.
1. Rivedere i risultati di diagnostica che mostrano i dettagli di quanto accaduto e delle misure da adottare per effettuare eventuali modifiche, se necessario.

**Verificare lo scenario applicabile:**

1. Se un utente non riceve una notifica push nell'app Microsoft Authenticator, verifica che non siano visualizzati sotto gli utenti bloccati dell'autenticazione a più fattori, come descritto in Bloccare e [sbloccare gli utenti](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).
1. Se l'utente non è bloccato per L'autenticazione a più fattori ma non riceve una notifica push, può aprire l'app Microsoft Authenticator, che estrarrà le richieste di approvazione in sospeso.
1. Come metodo di accesso alternativo, l'utente può anche fare clic su Accedi in un altro modo e scegliere di usare un codice di verifica dalla mia app per dispositivi mobili.
1. L Microsoft Authenticator App è l'unico metodo disponibile per molti utenti. [Per altre informazioni sulle impostazioni predefinite di sicurezza,](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) [Authenticator domande frequenti](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) sulle app per le domande frequenti e su come risolverle.
 
**Video consigliati**

[Come configurare l'Authenticator app su un nuovo telefono (2 minuti).](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)
