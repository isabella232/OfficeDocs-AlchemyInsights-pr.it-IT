---
title: Messaggio che informa che non è stato trovato alcun abbonamento nel Security Center
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 777fb9b09aa26d166f9971589bda464ccb90f4be
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544112"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a><span data-ttu-id="fc282-102">Messaggio che informa che non è stato trovato alcun abbonamento nel Security Center</span><span class="sxs-lookup"><span data-stu-id="fc282-102">No subscriptions found message in the Security Center</span></span>

<span data-ttu-id="fc282-103">Se durante l'accesso a Microsoft Defender Security Center viene visualizzato il messaggio "Nessuna sottoscrizione trovata", l'istanza di Azure Active Directory (AAD) usata per consentire all'utente di accedere al portale non include una licenza di Microsoft Defender ATP.</span><span class="sxs-lookup"><span data-stu-id="fc282-103">If while accessing Microsoft Defender Security Center you get a "No subscriptions found" message, it means the Azure Active Directory (AAD) used to login the user to the portal doesn't have a Microsoft Defender ATP license.</span></span>  

<span data-ttu-id="fc282-104">Le licenze di Windows E5 e Office E5 sono licenze distinte.</span><span class="sxs-lookup"><span data-stu-id="fc282-104">The Windows E5 and Office E5 licenses are separate licenses.</span></span>

<span data-ttu-id="fc282-p101">Aprire un caso di supporto se la licenza è stata acquistata ma non è stato eseguito il provisioning all'istanza di AAD. Potrebbe essersi verificato quanto segue:</span><span class="sxs-lookup"><span data-stu-id="fc282-p101">Open a support case if the license was purchased but not provisioned to this AAD instance. Either you have:</span></span> <br/>
-   <span data-ttu-id="fc282-107">Un possibile problema di provisioning della licenza.</span><span class="sxs-lookup"><span data-stu-id="fc282-107">A possible license provisioning issue.</span></span><br/>
-   <span data-ttu-id="fc282-108">È stato eseguito inavvertitamente il provisioning della licenza a un Microsoft AAD differente rispetto a quello usato per l'autenticazione al servizio.</span><span class="sxs-lookup"><span data-stu-id="fc282-108">You inadvertently provisioned the license to a different Microsoft AAD than the one used for authentication into the service.</span></span>