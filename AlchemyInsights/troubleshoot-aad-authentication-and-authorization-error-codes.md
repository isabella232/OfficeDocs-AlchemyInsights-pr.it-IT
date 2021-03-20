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
ms.openlocfilehash: 14555dfcb1406fd3a3977012393714a713ff80dc
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 03/19/2021
ms.locfileid: "50898309"
---
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a><span data-ttu-id="2d8c0-102">Risolvere i problemi relativi ai codici di errore di autenticazione e autorizzazione di Azure AD (AADSTS)</span><span class="sxs-lookup"><span data-stu-id="2d8c0-102">Troubleshoot Azure AD Authentication and Authorization (AADSTS) error codes</span></span>

<span data-ttu-id="2d8c0-103">Pe risolvere i codici di errore di autenticazione e autorizzazione AAD (AADSTS), eseguire i seguenti passaggi consigliati:</span><span class="sxs-lookup"><span data-stu-id="2d8c0-103">To resolve AAD authentication and authorization error codes (AADSTS), perform the following recommended steps:</span></span>

1. <span data-ttu-id="2d8c0-104">**Gestione dei codici di errore nell’applicazione**</span><span class="sxs-lookup"><span data-stu-id="2d8c0-104">**Handling error codes in your application**</span></span>

- <span data-ttu-id="2d8c0-105">La **specifica OAuth2.0**, https://tools.ietf.org/html/rfc6749#section-5.2, fornisce indicazioni su come gestire gli errori durante l’autenticazione usando la parte di errore della risposta di errore.</span><span class="sxs-lookup"><span data-stu-id="2d8c0-105">The **OAuth2.0 spec**, https://tools.ietf.org/html/rfc6749#section-5.2, provides guidance on how to handle errors during authentication using the error portion of the error response.</span></span>

    - <span data-ttu-id="2d8c0-106">**errore**: una stringa di codice di errore che può essere usata per classificare i tipi di errori che si verificano e che deve essere usata per reagire agli errori.</span><span class="sxs-lookup"><span data-stu-id="2d8c0-106">**error**: An error code string that can be used to classify types of errors that occur, and should be used to react to errors.</span></span>
    - <span data-ttu-id="2d8c0-107">Il campo dell’ **errore** ha diversi valori possibili: consulta i collegamenti alla documentazione del protocollo e le specifiche OAuth 2.0 per ulteriori informazioni su errori specifici e su come reagire ad essi.</span><span class="sxs-lookup"><span data-stu-id="2d8c0-107">The **error** field has several possible values - review the protocol documentation links and OAuth 2.0 specs for more information about specific errors and how to react to them.</span></span>

- <span data-ttu-id="2d8c0-108">Ecco una risposta di errore di esempio:</span><span class="sxs-lookup"><span data-stu-id="2d8c0-108">Here is a sample error response:</span></span>
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
2. <span data-ttu-id="2d8c0-109">**Ricerca delle informazioni del codice di errore corrente**</span><span class="sxs-lookup"><span data-stu-id="2d8c0-109">**Lookup current error code information**</span></span>

- <span data-ttu-id="2d8c0-110">I codici di errore e i messaggi sono soggetti a modifiche.</span><span class="sxs-lookup"><span data-stu-id="2d8c0-110">Error codes and messages are subject to change.</span></span> <span data-ttu-id="2d8c0-111">Per le informazioni più recenti, vedere la pagina https://login.microsoftonline.com/error per trovare le descrizioni dell’errore AADSTS, le correzioni e alcune soluzioni alternative suggerite.</span><span class="sxs-lookup"><span data-stu-id="2d8c0-111">For the most current information, see the https://login.microsoftonline.com/error page to find AADSTS error descriptions, fixes, and some suggested workarounds.</span></span>
- <span data-ttu-id="2d8c0-112">Inoltre, è possibile cercare e risolvere i problemi relativi ai [codici di errore AADSTS](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) elencati nell’articolo [Codici di errore di autenticazione e autorizzazione di Azure AD](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).</span><span class="sxs-lookup"><span data-stu-id="2d8c0-112">You can also search for and troubleshoot [AADSTS error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) listed in the article [Azure AD Authentication and authorization error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).</span></span>

3. <span data-ttu-id="2d8c0-113">**Accedere a Guida e supporto**</span><span class="sxs-lookup"><span data-stu-id="2d8c0-113">**Get Help**</span></span>

- <span data-ttu-id="2d8c0-114">[Opzioni di supporto a aiuto per sviluppatori](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options): se ti serve una risposta a una domanda o aiuto per risolvere un problema non trattato nella nostra documentazione, potrebbe essere il momento di contattare gli esperti per ricevere assistenza.</span><span class="sxs-lookup"><span data-stu-id="2d8c0-114">[Support and help options for developers](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) - If you need an answer to a question or help in solving a problem not covered in our documentation, it might be time to reach out to experts for help.</span></span> <span data-ttu-id="2d8c0-115">Questo articolo fornisce diversi suggerimenti per ottenere risposte alle tue domande mentre sviluppi app che si integrano con Microsoft Identity Platform.</span><span class="sxs-lookup"><span data-stu-id="2d8c0-115">This article provides several suggestions for getting answers to your questions as you develop apps that integrate with the Microsoft identity platform.</span></span>








