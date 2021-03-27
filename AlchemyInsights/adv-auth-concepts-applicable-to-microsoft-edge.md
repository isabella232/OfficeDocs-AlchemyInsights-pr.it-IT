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
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="2379c-102">Concetti di autenticazione avanzata applicabili a Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="2379c-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="2379c-103">Di seguito sono riportati i concetti di autenticazione avanzata applicabili a Microsoft Edge:</span><span class="sxs-lookup"><span data-stu-id="2379c-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="2379c-104">**Autenticazione proattiva**</span><span class="sxs-lookup"><span data-stu-id="2379c-104">**Proactive Authentication**</span></span>

<span data-ttu-id="2379c-105">Quando abiliti il [criterio ProactiveAuthEnabled,](https://go.microsoft.com/fwlink/?linkid=2134621) Microsoft Edge tenterà di autenticare in modo proattivo gli utenti connessi tramite i servizi Microsoft.</span><span class="sxs-lookup"><span data-stu-id="2379c-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="2379c-106">A intervalli regolari, verrà utilizzato un servizio online per verificare la presenza di un manifesto aggiornato contenente la configurazione che regola l'autenticazione proattiva.</span><span class="sxs-lookup"><span data-stu-id="2379c-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="2379c-107">Vantaggi: l'autenticazione proattiva consente l'autenticazione a servizi chiave, ad esempio la pagina Nuova scheda di Office.</span><span class="sxs-lookup"><span data-stu-id="2379c-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="2379c-108">Inoltre, se Bing viene utilizzato come motore di ricerca, l'autenticazione proattiva migliora le prestazioni della barra degli indirizzi e consente di generare risultati di ricerca personalizzati in base alle esigenze dell'azienda.</span><span class="sxs-lookup"><span data-stu-id="2379c-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="2379c-109">**Windows Hello CredUI per l'autenticazione NTLM**</span><span class="sxs-lookup"><span data-stu-id="2379c-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="2379c-110">Se single sign-on (SSO) non è disponibile quando un sito Web tenta di accedere all'utente tramite il meccanismo NTLM o Negotiate, questa funzionalità consentirà all'utente di condividere le credenziali del sistema operativo con il sito Web e di soddisfare la richiesta di autenticazione tramite l'interfaccia utente di Windows Hello Cred.</span><span class="sxs-lookup"><span data-stu-id="2379c-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="2379c-111">Questo flusso di accesso verrà visualizzato solo in Windows 10 e solo per gli utenti che non ottengono SSO durante una verifica NTLM o Negozia.</span><span class="sxs-lookup"><span data-stu-id="2379c-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="2379c-112">**Usare le password salvate per accedere automaticamente**</span><span class="sxs-lookup"><span data-stu-id="2379c-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="2379c-113">Gli utenti che salvano le password in Microsoft Edge possono abilitare l'accesso automatico ai siti Web in cui hanno salvato le credenziali.</span><span class="sxs-lookup"><span data-stu-id="2379c-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="2379c-114">Gli utenti possono attivare o disattivare questa funzionalità in edge://settings/passwords ed è possibile configurarla nei criteri di [gestione delle password.](https://go.microsoft.com/fwlink/?linkid=2134622)</span><span class="sxs-lookup"><span data-stu-id="2379c-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
