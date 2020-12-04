---
title: Concetti di autenticazione avanzata applicabili a Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
ms.openlocfilehash: 241d594fac6664dd1e85fd60e30a6344c432555e
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/04/2020
ms.locfileid: "49571890"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Concetti di autenticazione avanzata applicabili a Microsoft Edge

Di seguito sono riportati i concetti di autenticazione avanzati applicabili a Microsoft Edge:

**Autenticazione proattiva**

Quando si Abilita il criterio [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) , Microsoft Edge tenterà di autenticare in modo proattivo gli utenti che hanno eseguito l'accesso tramite i servizi Microsoft. A intervalli regolari, utilizzerà un servizio online per verificare l'utilizzo di un manifesto aggiornato che contenga la configurazione che disciplina l'autenticazione proattiva.

Vantaggi: l'autenticazione proattiva consente l'autenticazione ai servizi chiave, ad esempio la pagina nuova scheda Office. Inoltre, se viene utilizzato Bing come motore di ricerca, l'autenticazione proattiva migliora le prestazioni della barra degli indirizzi e consente di generare i risultati della ricerca personalizzati per le esigenze dell'azienda.

**Windows Hello CredUI per l'autenticazione NTLM**

Se Single Sign-on (SSO) non è disponibile quando un sito Web tenta di accedere all'utente tramite il meccanismo NTLM o Negotiate, questa funzionalità consente all'utente di condividere le credenziali del sistema operativo con il sito Web e di soddisfare la sfida di autenticazione utilizzando l'interfaccia utente di Windows Hello cred. Questo flusso di accesso verrà visualizzato solo in Windows 10 e solo per gli utenti che non ottengono SSO durante una sfida NTLM o Negotiate.

**Utilizzare le password salvate per eseguire l'accesso automatico**

Gli utenti che salvano le password in Microsoft Edge possono abilitare l'accesso automatico ai siti Web in cui sono state salvate le credenziali. Gli utenti possono abilitare o disabilitare questa funzionalità in edge://settings/passwords ed è possibile configurarla nei criteri di [gestione delle password](https://go.microsoft.com/fwlink/?linkid=2134622) .
