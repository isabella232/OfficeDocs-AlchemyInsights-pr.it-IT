---
title: 726 blocco dell'inoltro della posta elettronica
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: c0d9ed14f83d3c7d47e1728d5ed9ca3a19412ad2
ms.sourcegitcommit: f74c9698a31634154ce58dda8b3145bb10685ace
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/23/2020
ms.locfileid: "48219859"
---
# <a name="blocking-or-unblocking-email-forwarding"></a><span data-ttu-id="530b9-102">Blocco o sblocco dell'inoltro della posta elettronica</span><span class="sxs-lookup"><span data-stu-id="530b9-102">Blocking or unblocking email forwarding</span></span>

<span data-ttu-id="530b9-103">Per abilitare o disabilitare l'inoltro della posta elettronica per una cassetta postale specifica, vedere [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="530b9-103">To enable or disable email forwarding for a specific mailbox, see [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>

<span data-ttu-id="530b9-104">A livello di tenant, il controllo dell'inoltro esterno viene effettuato utilizzando il criterio di protezione dalla posta indesiderata in uscita.</span><span class="sxs-lookup"><span data-stu-id="530b9-104">On the tenant level, control of External forwarding is done using the outbound anti-spam policy.</span></span> <span data-ttu-id="530b9-105">Se è impostato su disattivato o automatico, potrebbe bloccare l'inoltro della posta elettronica con il messaggio di errore "550 5.7.520 Access Denied, l'organizzazione non consente l'inoltro esterno".</span><span class="sxs-lookup"><span data-stu-id="530b9-105">If it is set to Off or Automatic, it might block email forwarding with the “550 5.7.520 Access denied, Your organization does not allow external forwarding” error.</span></span> <span data-ttu-id="530b9-106">Successivamente, se l'inoltro è stato impostato per essere bloccato, questo è l'errore che vedranno gli utenti.</span><span class="sxs-lookup"><span data-stu-id="530b9-106">Subsequently, if forwarding was set to be blocked, that is the error your users will see.</span></span>

<span data-ttu-id="530b9-107">Se l'inoltro viene bloccato, verificare che i criteri siano configurati per abilitare l'inoltro AutoForward esterno.</span><span class="sxs-lookup"><span data-stu-id="530b9-107">If forwarding is being blocked, please make sure the policy is configured to enable External Autoforward.</span></span> <span data-ttu-id="530b9-108">È possibile controllare il criterio del filtro della posta indesiderata in uscita dal centro sicurezza e conformità o eseguendo il comando Get-HostedOutboundSpamFilterPolicy | nome FL, AutoForwardingMode.</span><span class="sxs-lookup"><span data-stu-id="530b9-108">You can check the Outbound Spam Filter Policy from Security and Compliance Center or by running command Get-HostedOutboundSpamFilterPolicy | fl name,AutoForwardingMode.</span></span> <span data-ttu-id="530b9-109">Se si desidera configurare il blocco AutoForward, lo stesso comando diranno lo stato dei criteri ora.</span><span class="sxs-lookup"><span data-stu-id="530b9-109">If you want to set up Autoforward blocking, the same command will tell you the state of policy now.</span></span>

<span data-ttu-id="530b9-110">Nota: si consiglia di mantenere disattivata l'AutoForward esterno sui criteri di filtro della posta indesiderata in uscita predefiniti e di abilitarla solo per gli utenti che hanno bisogno di un inoltro esterno creando un criterio personalizzato per tali utenti.</span><span class="sxs-lookup"><span data-stu-id="530b9-110">Note: It is recommended to keep the External Autoforward disabled on your Default Outbound Spam Filter Policy and enable it only for the users who need external forwarding by creating a custom policy for those users.</span></span> <span data-ttu-id="530b9-111">Per ulteriori informazioni, vedere [configurazione dell'inoltro della posta elettronica esterno in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="530b9-111">You can read more in [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span></span>