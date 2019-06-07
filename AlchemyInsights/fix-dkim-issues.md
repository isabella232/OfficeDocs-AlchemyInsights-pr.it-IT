---
title: Risolvere i problemi di installazione di DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 4d6dadbcbf71fe6e9ea56d6a82a7d8ababdd38ef
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765175"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="12fda-102">Risolvere i problemi di installazione di DKIM</span><span class="sxs-lookup"><span data-stu-id="12fda-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="12fda-103">Se si verificano problemi per l'abilitazione di DKIM per il dominio personalizzato, attenersi alla procedura seguente:</span><span class="sxs-lookup"><span data-stu-id="12fda-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="12fda-104">La maggior parte dei problemi di installazione di DKIM è correlata a record DNS non corretti.</span><span class="sxs-lookup"><span data-stu-id="12fda-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="12fda-105">Verificare che il record CNAME di DKIM (**non** un record TXT) sia formattato correttamente.</span><span class="sxs-lookup"><span data-stu-id="12fda-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="12fda-106">Per ulteriori informazioni, vedere questo [argomento](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="12fda-106">For more information, see this [topic](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

- <span data-ttu-id="12fda-107">Dopo aver creato o aggiornato i record DNS di DKIM nel servizio di hosting DNS per il dominio (in genere, il registrar), attendere che i record DNS vengano propagati.</span><span class="sxs-lookup"><span data-stu-id="12fda-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="12fda-108">Se non è possibile creare i record DNS di DKIM nell'interfaccia di amministrazione, è \<possibile\> sostituire CustomDomain con il dominio personalizzato, ad esempio contoso.com, ed eseguire questo comando in [PowerShell di Exchange Online](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span><span class="sxs-lookup"><span data-stu-id="12fda-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
