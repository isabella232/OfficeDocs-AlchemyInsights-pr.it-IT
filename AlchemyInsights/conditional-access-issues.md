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
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013952"
---
# <a name="conditional-access-issues"></a>Problemi di accesso condizionale

**Risolvere i problemi con la diagnostica di accesso**

È possibile scoprire rapidamente cosa è successo o diagnosticare i problemi relativi all'accesso dell'utente utilizzando la [diagnostica di accesso](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):

1. Avviare la Diagnostica di accesso.
1. Individuare l'evento da analizzare immettendo i dettagli sull'utente, l'applicazione, l'ora di accesso, l'ID richiesta o l'ID di correlazione.
1. Esaminare i risultati diagnostici in cui vengono illustrati i dettagli relativi a ciò che è accaduto e le azioni che è possibile eseguire per apportare modifiche (se sono necessarie modifiche).

**Passaggi per la risoluzione dei problemi di accesso** 

1. Passare alla pagina di accesso di Azure AD.
1. Filtrare gli accessi in base all'utente, l'intervallo di tempo, l'applicazione, lo stato, l'app client e così via.
1. Selezionare un evento di accesso e visualizzare la scheda Access condizionale per vedere quali criteri sono stati valutati.
1. Fare clic sulla riga di un criterio per visualizzare i dettagli del criterio e comprendere il motivo per cui è stata applicata.

**Strumenti per la risoluzione di un criterio di accesso condizionale**

- La modalità solo report consente di valutare un criterio senza influire sugli utenti.
- Lo strumento What-If consente di simulare gli eventi di accesso e di vedere quali criteri si applicano.
- La cartella di lavoro Insights and Reporting Visualizza l'impatto in tempo reale di ogni criterio.

**Criteri di protezione di base**

I criteri di protezione di base sono stati deprecati. Non vengono più applicate e verranno presto rimossi dal portale di Azure. È consigliabile abilitare le [impostazioni predefinite](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)per la sicurezza.

Per ulteriori informazioni sull'accesso condizionale, vedere:

[Procedure consigliate per l'accesso condizionale in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Condizioni per l'accesso](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 condizionale [Controlli in accesso](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 condizionale [Posizioni in accesso condizionale](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)
