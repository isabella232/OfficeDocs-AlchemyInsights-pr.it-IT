---
title: Antispam - 5.7.23
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: e494e8017f24d65a94d1a7490be4d67c46a2120b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821415"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="ebeff-102">Risolvere i problemi di recapito della posta elettronica per il codice di errore 5.7.23</span><span class="sxs-lookup"><span data-stu-id="ebeff-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="ebeff-103">Verificare il record DNS SPF per il dominio in un controllo record SPF o DNS disponibile pubblicamente sul Web.</span><span class="sxs-lookup"><span data-stu-id="ebeff-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="ebeff-104">Verificare che il messaggio in uscita non sia stato identificato come posta indesiderata da Microsoft e instradato tramite [il pool di recapito ad alto rischio.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages)</span><span class="sxs-lookup"><span data-stu-id="ebeff-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="ebeff-105">I messaggi nel pool di recapito ad alto rischio non supereranno i controlli SPF e pertanto non verranno accettati dall'organizzazione di posta elettronica di destinazione.</span><span class="sxs-lookup"><span data-stu-id="ebeff-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="ebeff-106">Se il problema persiste, potrebbe essere necessario contattare l'amministratore dell'host di posta a cui si sta tentando di inviare posta elettronica.</span><span class="sxs-lookup"><span data-stu-id="ebeff-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="ebeff-107">Prendere nota dell'errore esterno dettagliato disponibile nel messaggio di mancato recapito.</span><span class="sxs-lookup"><span data-stu-id="ebeff-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="ebeff-108">Il supporto Tecnico Microsoft potrebbe non essere in grado di fornire ulteriore assistenza.</span><span class="sxs-lookup"><span data-stu-id="ebeff-108">Microsoft support may not be able to assist further.</span></span>
