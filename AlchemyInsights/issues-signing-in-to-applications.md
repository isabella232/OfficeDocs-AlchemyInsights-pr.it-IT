---
title: Problemi relativi all'accesso alle applicazioni
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7788"
- "9004355"
ms.openlocfilehash: 2d073367dc1c3e8e117c0b68e205297a65024872
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 01/18/2021
ms.locfileid: "49886849"
---
# <a name="issues-signing-in-to-applications"></a>Problemi relativi all'accesso alle applicazioni

Per rilevare la causa o i problemi di diagnostica correlati all'accesso utente, seguire questi passaggi:

1. Avviare la [Diagnostica di accesso](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).
2. Trovare l'evento da analizzare inserendo i dettagli di cui si dispone in merito a utente, applicazione, ora di accesso, ID richiesta o ID correlazione.
3. Rivedere i risultati di diagnostica che mostrano i dettagli di quanto accaduto e delle misure da adottare per effettuare eventuali modifiche, se necessario.

Seguono alcuni problemi comuni che si potrebbero riscontrare durante l'accesso alle applicazioni:

1. **È stato completato un accesso ad Azure AD, ma viene visualizzata una richiesta imprevista** - Vedere gli articoli [Richiesta di consenso imprevista durante l'accesso a un'applicazione](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt) ed [Errore imprevisto durante la fornitura del consenso a un'applicazione](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).
2. **È stato eseguito l'accesso direttamente a un'applicazione, ma non è possibile accedere da un collegamento diretto sul portale personalizzato o nel riquadro di accesso**: vedere [Risolvere i problemi relativi all'accesso a un'applicazione da Mie app di Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel).
3. **È stato completato l'accesso ad Azure AD, ma l'applicazione mostra un messaggio di errore e non consente all'utente di completare il flusso di accesso**: il problema risiede nel fatto che l'app non ha accettato la risposta emessa da Azure AD. Seguire [questi passaggi](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-application-error) per la risoluzione dei problemi.
4. **Impossibile accedere a un'applicazione non nella raccolta configurata per il Single Sign-On delle password**: seguire le linee guida presenti in [questi passaggi](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) per la risoluzione dei problemi.
5. **Impossibile accedere a un'applicazione nella raccolta di Azure AD configurata per il Single Sign-On delle password**: seguire [questi passaggi](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) per la risoluzione dei problemi.
6. **Impossibile accedere a un'applicazione Microsoft**: seguire [questi passaggi](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft) per la risoluzione dei problemi.
7. **Impossibile accedere a un'applicazione non nella raccolta configurata per il Single Sign-On federato**: seguire [questi passaggi](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-federated-sso-non-gallery) per la risoluzione dei problemi.
8. **Impossibile accedere a un'applicazione nella raccolta di Azure AD configurata per il Single Sign-On federato**: seguire [questi passaggi](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) per la risoluzione dei problemi.
9. **Impossibile accedere a un'applicazione personalizzata**: seguire [questi passaggi](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) per la risoluzione dei problemi.
10. **Impossibile accedere a un'applicazione locale tramite il proxy di autenticazione di Azure AD**: seguire [questi passaggi](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-on-premises-application-proxy) per la risoluzione dei problemi.

