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
ms.openlocfilehash: 610013c4f46e999f1a8715aea14dd557ed8b0e2a
ms.sourcegitcommit: 88f24bb6ced16842de165af416e3f21feae13063
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 10/15/2020
ms.locfileid: "48478316"
---
# <a name="blocking-or-unblocking-email-forwarding"></a><span data-ttu-id="1acfc-102">Blocco o sblocco dell'inoltro della posta elettronica</span><span class="sxs-lookup"><span data-stu-id="1acfc-102">Blocking or unblocking email forwarding</span></span>

<span data-ttu-id="1acfc-103">Per abilitare o disabilitare l'inoltro della posta elettronica per una cassetta postale specifica, vedere [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="1acfc-103">To enable or disable email forwarding for a specific mailbox, see [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>

<span data-ttu-id="1acfc-104">A livello di tenant, il controllo dell'inoltro esterno viene effettuato utilizzando il criterio della posta indesiderata in uscita.</span><span class="sxs-lookup"><span data-stu-id="1acfc-104">On the tenant level, control of external forwarding is done using the outbound spam policy.</span></span> <span data-ttu-id="1acfc-105">È possibile controllare il criterio dei filtri per la posta indesiderata in uscita dal centro sicurezza e conformità [qui](https://protection.office.com/antispam) o utilizzando il [comando Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).</span><span class="sxs-lookup"><span data-stu-id="1acfc-105">You can check the outbound spam filter policy from Security and Compliance Center [here](https://protection.office.com/antispam) or by using the [Get-HostedOutboundSpamFilterPolicy command](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).</span></span>

<span data-ttu-id="1acfc-106">Se viene visualizzato il messaggio di errore seguente: **"550 5.7.520 accesso negato, l'organizzazione non consente l'inoltro esterno"**, verificare che il criterio sia configurato per abilitare l'inoltro automatico esterno.</span><span class="sxs-lookup"><span data-stu-id="1acfc-106">If you are getting the following error: **“550 5.7.520 Access denied, Your organization does not allow external forwarding”**, please make sure the policy is configured to enable External Auto-forward.</span></span>

<span data-ttu-id="1acfc-107">**Nota:** Si consiglia di mantenere disattivata l'AutoForward esterno sui criteri di filtro della posta indesiderata in uscita predefiniti e di abilitarla solo per gli utenti che hanno bisogno di un inoltro esterno creando un criterio personalizzato per tali utenti.</span><span class="sxs-lookup"><span data-stu-id="1acfc-107">**Note:** It is recommended to keep the External Autoforward disabled on your default outbound spam filter policy and enable it only for the users who need external forwarding by creating a custom policy for those users.</span></span> <span data-ttu-id="1acfc-108">Per ulteriori informazioni, vedere [configurazione dell'inoltro della posta elettronica esterno in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="1acfc-108">You can read more in [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span></span>