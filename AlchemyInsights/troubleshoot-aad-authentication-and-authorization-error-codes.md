---
title: Risolvere i problemi relativi ai codici di errore di autenticazione e autorizzazione di Azure AD (AADSTS)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9800"
- "9005744"
ms.openlocfilehash: ac25548b0110834c877ae53be097d6b6c0f13c4091040a901abd56fb2a3cbba3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939959"
---
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a>Risolvere i problemi relativi ai codici di errore di autenticazione e autorizzazione di Azure AD (AADSTS)

Pe risolvere i codici di errore di autenticazione e autorizzazione AAD (AADSTS), eseguire i seguenti passaggi consigliati:

1. **Gestione dei codici di errore nell’applicazione**

- La **specifica OAuth2.0**, https://tools.ietf.org/html/rfc6749#section-5.2, fornisce indicazioni su come gestire gli errori durante l’autenticazione usando la parte di errore della risposta di errore.

    - **errore**: una stringa di codice di errore che può essere usata per classificare i tipi di errori che si verificano e che deve essere usata per reagire agli errori.
    - Il campo dell’ **errore** ha diversi valori possibili: consulta i collegamenti alla documentazione del protocollo e le specifiche OAuth 2.0 per ulteriori informazioni su errori specifici e su come reagire ad essi.

- Ecco una risposta di errore di esempio:
```
{
  "error": "invalid_scope",
  "error_description": "AADSTS70011: The provided value for the input parameter 'scope' is not 
valid. The scope https://example.contoso.com/activity.read is not valid.\r\nTrace ID: 255d1aef- 8c98-452f-ac51-23d051240864\r\nCorrelation ID: fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7\r\nTimestamp: 2016-01-09 02:02:12Z",
  "error_codes": [
    70011
  ],
  "timestamp": "2016-01-09 02:02:12Z",
  "trace_id": "255d1aef-8c98-452f-ac51-23d051240864",
  "correlation_id": "fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7", 
  "error_uri":"https://login.microsoftonline.com/error?code=70011"
}
```
2. **Ricerca delle informazioni del codice di errore corrente**

- I codici e i messaggi di errore sono soggetti a variazione. Per le informazioni più recenti, vedere la pagina https://login.microsoftonline.com/error per trovare le descrizioni dell’errore AADSTS, le correzioni e alcune soluzioni alternative suggerite.
- Inoltre, è possibile cercare e risolvere i problemi relativi ai [codici di errore AADSTS](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) elencati nell’articolo [Codici di errore di autenticazione e autorizzazione di Azure AD](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).

3. **Accedere a Guida e supporto**

- [Opzioni di supporto a aiuto per sviluppatori](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options): se ti serve una risposta a una domanda o aiuto per risolvere un problema non trattato nella nostra documentazione, potrebbe essere il momento di contattare gli esperti per ricevere assistenza. Questo articolo fornisce diversi suggerimenti per ottenere risposte alle tue domande mentre sviluppi app che si integrano con Microsoft Identity Platform.








