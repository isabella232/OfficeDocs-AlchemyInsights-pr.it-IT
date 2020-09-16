---
title: Risolvere i problemi di installazione di DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 35e8023d26fe26211e27521ceb8751d2d7fc7a21
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744954"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="03518-102">Risolvere i problemi di installazione di DKIM</span><span class="sxs-lookup"><span data-stu-id="03518-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="03518-103">Se si verificano problemi per l'abilitazione di DKIM per il dominio personalizzato, attenersi alla procedura seguente:</span><span class="sxs-lookup"><span data-stu-id="03518-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="03518-104">La maggior parte dei problemi di installazione di DKIM è correlata a record DNS non corretti.</span><span class="sxs-lookup"><span data-stu-id="03518-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="03518-105">Verificare che il record CNAME di DKIM (**non** un record TXT) sia formattato correttamente.</span><span class="sxs-lookup"><span data-stu-id="03518-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="03518-106">Per ulteriori informazioni, vedere questo [argomento](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span><span class="sxs-lookup"><span data-stu-id="03518-106">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

- <span data-ttu-id="03518-107">Dopo aver creato o aggiornato i record DNS di DKIM nel servizio di hosting DNS per il dominio (in genere, il registrar), attendere che i record DNS vengano propagati.</span><span class="sxs-lookup"><span data-stu-id="03518-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="03518-108">Se non è possibile creare i record DNS di DKIM nell'interfaccia di amministrazione, è possibile sostituirli \<CustomDomain\> con il dominio personalizzato (ad esempio, contoso.com) ed eseguire questo comando in [PowerShell di Exchange Online](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .</span><span class="sxs-lookup"><span data-stu-id="03518-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
