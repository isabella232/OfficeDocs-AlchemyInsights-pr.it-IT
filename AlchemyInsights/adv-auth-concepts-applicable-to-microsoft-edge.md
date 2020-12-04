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
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="d3421-102">Concetti di autenticazione avanzata applicabili a Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="d3421-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="d3421-103">Di seguito sono riportati i concetti di autenticazione avanzati applicabili a Microsoft Edge:</span><span class="sxs-lookup"><span data-stu-id="d3421-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="d3421-104">**Autenticazione proattiva**</span><span class="sxs-lookup"><span data-stu-id="d3421-104">**Proactive Authentication**</span></span>

<span data-ttu-id="d3421-105">Quando si Abilita il criterio [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) , Microsoft Edge tenterà di autenticare in modo proattivo gli utenti che hanno eseguito l'accesso tramite i servizi Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d3421-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="d3421-106">A intervalli regolari, utilizzerà un servizio online per verificare l'utilizzo di un manifesto aggiornato che contenga la configurazione che disciplina l'autenticazione proattiva.</span><span class="sxs-lookup"><span data-stu-id="d3421-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="d3421-107">Vantaggi: l'autenticazione proattiva consente l'autenticazione ai servizi chiave, ad esempio la pagina nuova scheda Office.</span><span class="sxs-lookup"><span data-stu-id="d3421-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="d3421-108">Inoltre, se viene utilizzato Bing come motore di ricerca, l'autenticazione proattiva migliora le prestazioni della barra degli indirizzi e consente di generare i risultati della ricerca personalizzati per le esigenze dell'azienda.</span><span class="sxs-lookup"><span data-stu-id="d3421-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="d3421-109">**Windows Hello CredUI per l'autenticazione NTLM**</span><span class="sxs-lookup"><span data-stu-id="d3421-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="d3421-110">Se Single Sign-on (SSO) non è disponibile quando un sito Web tenta di accedere all'utente tramite il meccanismo NTLM o Negotiate, questa funzionalità consente all'utente di condividere le credenziali del sistema operativo con il sito Web e di soddisfare la sfida di autenticazione utilizzando l'interfaccia utente di Windows Hello cred.</span><span class="sxs-lookup"><span data-stu-id="d3421-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="d3421-111">Questo flusso di accesso verrà visualizzato solo in Windows 10 e solo per gli utenti che non ottengono SSO durante una sfida NTLM o Negotiate.</span><span class="sxs-lookup"><span data-stu-id="d3421-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="d3421-112">**Utilizzare le password salvate per eseguire l'accesso automatico**</span><span class="sxs-lookup"><span data-stu-id="d3421-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="d3421-113">Gli utenti che salvano le password in Microsoft Edge possono abilitare l'accesso automatico ai siti Web in cui sono state salvate le credenziali.</span><span class="sxs-lookup"><span data-stu-id="d3421-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="d3421-114">Gli utenti possono abilitare o disabilitare questa funzionalità in edge://settings/passwords ed è possibile configurarla nei criteri di [gestione delle password](https://go.microsoft.com/fwlink/?linkid=2134622) .</span><span class="sxs-lookup"><span data-stu-id="d3421-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
