---
title: Pool di inoltro in uscita
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "12315"
ms.openlocfilehash: b723566a29e0be581b7fdc30332166d5cddbd38f
ms.sourcegitcommit: 270a1ca9c35b50b8be6b06f432c9c90e4090fb57
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/08/2021
ms.locfileid: "53339980"
---
# <a name="outbound-relay-pool"></a><span data-ttu-id="11a11-102">Pool di inoltro in uscita</span><span class="sxs-lookup"><span data-stu-id="11a11-102">Outbound relay pool</span></span>

<span data-ttu-id="11a11-103">Microsoft sta apportando alcune modifiche alla configurazione per l'inoltro o l'inoltro della posta elettronica tramite Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="11a11-103">Microsoft is making some changes to the configuration for relaying or forwarding email through Microsoft 365.</span></span> <span data-ttu-id="11a11-104">I messaggi in determinati scenari vengono inoltrati o inoltrati tramite Microsoft 365 utilizzando uno speciale pool di inoltro.</span><span class="sxs-lookup"><span data-stu-id="11a11-104">Messages in certain scenarios are forwarded or relayed through Microsoft 365 using a special relay pool.</span></span> <span data-ttu-id="11a11-105">I messaggi inviati utilizzando il pool di inoltro potrebbero finire nella cartella posta indesiderata del destinatario.</span><span class="sxs-lookup"><span data-stu-id="11a11-105">Messages sent by using the relay pool could end up in recipient's junk mail folder.</span></span> <span data-ttu-id="11a11-106">Per ulteriori informazioni, vedere [Outbound delivery pools](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span><span class="sxs-lookup"><span data-stu-id="11a11-106">For more information, see [Outbound delivery pools](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span></span>

<span data-ttu-id="11a11-107">Per evitare uno scenario che utilizza il pool di inoltro, verificare che i messaggi inoltrati/inoltrati soddisfino uno dei criteri seguenti:</span><span class="sxs-lookup"><span data-stu-id="11a11-107">To avoid a scenario using the relay pool, make sure that forwarded/relayed messages meet one of the following criteria:</span></span>

- <span data-ttu-id="11a11-108">Il mittente in uscita è un dominio accettato del tenant.</span><span class="sxs-lookup"><span data-stu-id="11a11-108">The outbound sender is an accepted domain of the tenant.</span></span>
- <span data-ttu-id="11a11-109">Sender Policy Framework (SPF) passa quando il messaggio Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="11a11-109">Sender Policy Framework (SPF) passes when the message comes to Microsoft 365.</span></span>
- <span data-ttu-id="11a11-110">DomainKeys Identified Mail (DKIM) nel dominio del mittente P2 passa quando il messaggio Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="11a11-110">DomainKeys Identified Mail (DKIM) on the P2 sender domain passes when the message comes to Microsoft 365.</span></span>
 
<span data-ttu-id="11a11-111">I messaggi che soddisfano i criteri precedenti non vengono inoltrati tramite il pool di inoltro.</span><span class="sxs-lookup"><span data-stu-id="11a11-111">Messages that meet the above criteria are not relayed through the relay pool.</span></span>

<span data-ttu-id="11a11-112">Se il record MX per il dominio fa riferimento a un server di terze parti o locale, utilizzare il filtro avanzato per verificare che la convalida SPF sia corretta per la posta elettronica in ingresso ed evitare di inviare posta elettronica tramite il pool di inoltro.</span><span class="sxs-lookup"><span data-stu-id="11a11-112">If the MX record for your domain is pointed to a third-party or on-premises server, use enhanced filtering to make sure the SPF validation is correct for inbound email and to avoid sending email through the relay pool.</span></span>

<span data-ttu-id="11a11-113">**Come è possibile determinare se il pool di inoltro è in grado di influire su di noi?**</span><span class="sxs-lookup"><span data-stu-id="11a11-113">**How can we tell if we're impacted by the relay pool?**</span></span>

<span data-ttu-id="11a11-114">Se i messaggi di posta elettronica inoltrati o inoltrati utilizzano uno dei criteri precedenti, i messaggi non verranno inoltrati tramite il pool di inoltro.</span><span class="sxs-lookup"><span data-stu-id="11a11-114">If your forwarded or relayed emails use one of the above criteria, messages won't be relayed through the relay pool.</span></span> <span data-ttu-id="11a11-115">Tuttavia, se un messaggio viene inviato tramite un pool di inoltro, l'IP del server in uscita si trova nell'intervallo 40.95.0.0/16 e il nome del server in uscita include **rly** nel nome.</span><span class="sxs-lookup"><span data-stu-id="11a11-115">However, if a message is sent through a relay pool, the outbound server IP is in the 40.95.0.0/16 range and the outbound server name includes **rly** in the name.</span></span>

