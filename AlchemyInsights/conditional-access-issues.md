---
title: Problemi di accesso condizionale
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7768"
ms.openlocfilehash: 85cbd89e461f36a51eed816619fd132ea60dfdb0014eb850c7ec3f38d41e1ca2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069968"
---
# <a name="conditional-access-issues"></a>Problemi di accesso condizionale

**Risolvere i problemi con la diagnostica di accesso**

Puoi scoprire rapidamente cosa è successo o diagnosticare i problemi relativi all'accesso utente usando Diagnostica [accesso:](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. Avviare la Diagnostica di accesso.
1. Trova l'evento da analizzare immettendo i dettagli relativi all'utente, all'applicazione, all'ora di accesso, all'ID richiesta o all'ID correlazione.
1. Esaminare i risultati di diagnostica che mostrano i dettagli dell'evento e le azioni che è possibile eseguire per apportare modifiche (se sono necessarie modifiche).

**Procedura per la risoluzione dei problemi di accesso** 

1. Passare alla pagina di accesso di Azure AD.
1. Filtra gli accesso per utente, intervallo di tempo, applicazione, stato, app client e così via.
1. Selezionare un evento di accesso e visualizzare la scheda Accesso condizionale per vedere quali criteri sono stati valutati.
1. Fare clic sulla riga di un criterio per visualizzare i dettagli del criterio e comprendere il motivo per cui è stato applicato.

**Strumenti per la risoluzione dei problemi di un criterio di accesso condizionale**

- La modalità solo report consente di valutare un criterio senza influire sugli utenti.
- Lo strumento di simulazione consente di simulare gli eventi di accesso e di vedere quali criteri si applicano.
- Insights cartella di lavoro per la creazione di report viene visualizzato l'impatto in tempo reale di ogni criterio.

**Criteri di protezione di base**

I criteri di protezione di base sono stati deprecati. Non vengono più applicati e verranno presto rimossi dal portale di Azure. È consigliabile abilitare [le impostazioni predefinite di sicurezza](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).

Per ulteriori informazioni sull'accesso condizionale, vedere:

[Procedure consigliate per l'accesso condizionale in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Condizioni nell'accesso condizionale](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Controlli nell'accesso condizionale](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Posizioni nell'accesso condizionale](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)
