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
ms.openlocfilehash: 01117bc535df14533e426fd2d31c336fccc75611
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/15/2020
ms.locfileid: "49768526"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a><span data-ttu-id="87482-102">Messaggio che informa che non è stato trovato alcun abbonamento nel Security Center</span><span class="sxs-lookup"><span data-stu-id="87482-102">No subscriptions found message in the Security Center</span></span>

<span data-ttu-id="87482-103">Se durante l'accesso al Microsoft Defender Security Center viene visualizzato il messaggio "Non è stato trovato alcun abbonamento", significa che Azure Active Directory (AAD) usato per far accedere l'utente al portale non dispone di una licenza di Microsoft Defender ATP.</span><span class="sxs-lookup"><span data-stu-id="87482-103">If while accessing Microsoft Defender Security Center you get a  "No subscriptions found" message, it means the Azure Active Directory (AAD) used to login the user to the portal doesn't have a Microsoft Defender ATP license.</span></span>  

<span data-ttu-id="87482-104">Le licenze di Windows E5 e Office E5 sono licenze distinte.</span><span class="sxs-lookup"><span data-stu-id="87482-104">The Windows E5 and Office E5 licenses are separate licenses.</span></span>

<span data-ttu-id="87482-105">Aprire un caso di supporto se la licenza è stata acquistata ma non è stato eseguito il provisioning all'istanza di AAD.</span><span class="sxs-lookup"><span data-stu-id="87482-105">Open a support case if the license was purchased but not provisioned to this AAD instance.</span></span> <span data-ttu-id="87482-106">Potrebbe essersi verificato quanto segue:</span><span class="sxs-lookup"><span data-stu-id="87482-106">Either you have:</span></span> <br/>
-   <span data-ttu-id="87482-107">Un possibile problema di provisioning della licenza.</span><span class="sxs-lookup"><span data-stu-id="87482-107">A possible license provisioning issue.</span></span><br/>
-   <span data-ttu-id="87482-108">È stato eseguito inavvertitamente il provisioning della licenza a un Microsoft AAD differente rispetto a quello usato per l'autenticazione al servizio.</span><span class="sxs-lookup"><span data-stu-id="87482-108">You inadvertently provisioned the license to a different Microsoft AAD than the one used for authentication into the service.</span></span>