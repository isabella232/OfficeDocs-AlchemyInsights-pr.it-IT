---
title: Protezione da posta indesiderata-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 307b738c40c620d057e68eff7d218c8c9b5eb665
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676501"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="96a3a-102">Risolvere problemi di recapito della posta elettronica per il codice di errore 5.7.23</span><span class="sxs-lookup"><span data-stu-id="96a3a-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="96a3a-103">Verificare il record DNS SPF per il dominio in un controllo del record SPF o DNS disponibile pubblicamente sul Web.</span><span class="sxs-lookup"><span data-stu-id="96a3a-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="96a3a-104">Verificare che il messaggio in uscita non sia stato identificato come posta indesiderata da Microsoft e instradato attraverso il [pool di recapito ad alto rischio](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="96a3a-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="96a3a-105">I messaggi nel pool di recapito ad alto rischio non superano i controlli SPF e pertanto non verranno accettati dall'organizzazione di posta elettronica di destinazione.</span><span class="sxs-lookup"><span data-stu-id="96a3a-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="96a3a-106">Se il problema persiste, potrebbe essere necessario contattare l'amministratore dell'host di posta elettronica a cui si sta tentando di inviare messaggi di posta elettronica.</span><span class="sxs-lookup"><span data-stu-id="96a3a-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="96a3a-107">Prendere nota dell'errore esterno dettagliato disponibile nel messaggio di rimbalzo.</span><span class="sxs-lookup"><span data-stu-id="96a3a-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="96a3a-108">Il supporto tecnico Microsoft potrebbe non essere in grado di supportare ulteriormente.</span><span class="sxs-lookup"><span data-stu-id="96a3a-108">Microsoft support may not be able to assist further.</span></span>
