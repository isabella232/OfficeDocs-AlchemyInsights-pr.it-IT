---
title: Non è possibile accedere a Teams a causa di un errore autologon.microsoftazuread-sso.com:443
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 77049153939989d1c63789adfec0b494d047a6e4
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932041"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a><span data-ttu-id="222f2-102">Non è possibile accedere a Teams a causa di un errore autologon.microsoftazuread-sso dot com:443</span><span class="sxs-lookup"><span data-stu-id="222f2-102">Unable to log into Teams due to error autologon.microsoftazuread-sso dot com:443</span></span>

<span data-ttu-id="222f2-103">Se come autenticazione di Office 365 è abilitato l'accesso SSO facile, potrebbe essere necessario aggiungere l'URL "autologon.microsoftazuread-sso.com" ai siti Intranet.</span><span class="sxs-lookup"><span data-stu-id="222f2-103">If Seamless SSO is enabled as the O365 authentication, the URL "autologon.microsoftazuread-sso.com" may need to be added to Intranet Sites.</span></span>  <span data-ttu-id="222f2-104">Se in precedenza è stato aggiunto all'elenco Siti attendibili ed è in uso l'accesso SSO facile, deve essere rimosso dai siti attendibili.</span><span class="sxs-lookup"><span data-stu-id="222f2-104">If it has previously been added to Trusted Sites  and Seamless SSO is in use, it should be removed from Trusted Sites.</span></span>

<span data-ttu-id="222f2-105">Leggere l'[elenco di controllo per la risoluzione dei problemi dell'accesso SSO facile](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span><span class="sxs-lookup"><span data-stu-id="222f2-105">Please review the [Seamless SSO Troubleshooting Checklist](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span></span>

<span data-ttu-id="222f2-106">Seguire questa procedura per aggiungere un URL all'elenco dei siti Intranet:</span><span class="sxs-lookup"><span data-stu-id="222f2-106">Follow these steps to add a URL to Intranet Sites list:</span></span>

1. <span data-ttu-id="222f2-107">Aprire Internet Explorer facendo clic sul pulsante **Start**.</span><span class="sxs-lookup"><span data-stu-id="222f2-107">Open Internet Explorer by clicking the **Start** button.</span></span> <span data-ttu-id="222f2-108">Nella casella di ricerca digitare Internet Explorer e quindi nell'elenco dei risultati fare clic su **Internet Explorer**.</span><span class="sxs-lookup"><span data-stu-id="222f2-108">In the search box, type Internet Explorer, and then, in the list of results, click **Internet Explorer**.</span></span>
2. <span data-ttu-id="222f2-109">Fare clic su **Strumenti**, quindi su **Opzioni Internet**.</span><span class="sxs-lookup"><span data-stu-id="222f2-109">Click **Tools**, and then click **Internet options**.</span></span>
3. <span data-ttu-id="222f2-110">Fare clic sulla scheda **Sicurezza**.</span><span class="sxs-lookup"><span data-stu-id="222f2-110">Click the **Security** tab.</span></span>
4. <span data-ttu-id="222f2-111">A questo punto, fare clic su **Intranet locale**, sul pulsante **siti** e quindi sul pulsante **Avanzate**.</span><span class="sxs-lookup"><span data-stu-id="222f2-111">Now click on **Local Intranet sites** and then click on the **sites** button and then **Advanced** button.</span></span>
5. <span data-ttu-id="222f2-112">Immettere l'URL del sito Web e fare clic su **Aggiungi**.</span><span class="sxs-lookup"><span data-stu-id="222f2-112">Enter the Website URL and click **Add**.</span></span>
6. <span data-ttu-id="222f2-113">Al termine, fare clic su **Chiudi**.</span><span class="sxs-lookup"><span data-stu-id="222f2-113">When you are finished, click **Close**.</span></span>

<span data-ttu-id="222f2-114">Per altre informazioni, vedere la [documentazione per la distribuzione dell'accesso SSO facile per Office 365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (include il processo basato su criteri per aggiungere un URL ai siti Intranet nel passaggio 3).</span><span class="sxs-lookup"><span data-stu-id="222f2-114">For more information, see [Documentation for deploying Seamless SSO for O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (includes Policy-based process to add a URL to Intranet Sites in Step 3).</span></span>
