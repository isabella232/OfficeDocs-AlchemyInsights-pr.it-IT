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
- "8329"
- "9004625"
ms.openlocfilehash: d469973c4f8605b00d32f6f625eb5fdd17e8f390
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398588"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Concetti di autenticazione avanzata applicabili a Microsoft Edge

Di seguito sono riportati i concetti di autenticazione avanzata applicabili a Microsoft Edge:

**Autenticazione proattiva**

Quando abiliti il [criterio ProactiveAuthEnabled,](https://go.microsoft.com/fwlink/?linkid=2134621) Microsoft Edge tenterà di autenticare in modo proattivo gli utenti connessi tramite i servizi Microsoft. A intervalli regolari, verrà utilizzato un servizio online per verificare la presenza di un manifesto aggiornato contenente la configurazione che regola l'autenticazione proattiva.

Vantaggi: l'autenticazione proattiva consente l'autenticazione a servizi chiave, ad esempio la pagina Nuova scheda di Office. Inoltre, se Bing viene utilizzato come motore di ricerca, l'autenticazione proattiva migliora le prestazioni della barra degli indirizzi e consente di generare risultati di ricerca personalizzati in base alle esigenze dell'azienda.

**Windows Hello CredUI per l'autenticazione NTLM**

Se single sign-on (SSO) non è disponibile quando un sito Web tenta di accedere all'utente tramite il meccanismo NTLM o Negotiate, questa funzionalità consentirà all'utente di condividere le credenziali del sistema operativo con il sito Web e di soddisfare la richiesta di autenticazione tramite l'interfaccia utente di Windows Hello Cred. Questo flusso di accesso verrà visualizzato solo in Windows 10 e solo per gli utenti che non ottengono SSO durante una verifica NTLM o Negozia.

**Usare le password salvate per accedere automaticamente**

Gli utenti che salvano le password in Microsoft Edge possono abilitare l'accesso automatico ai siti Web in cui hanno salvato le credenziali. Gli utenti possono attivare o disattivare questa funzionalità in edge://settings/passwords ed è possibile configurarla nei criteri di [gestione delle password.](https://go.microsoft.com/fwlink/?linkid=2134622)
