---
title: Risolvere i problemi di installazione di DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: d725eb0d46dcbf1b5b6d77ca9f59fcafa5298bf1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43717566"
---
# <a name="fix-dkim-setup-issues"></a>Risolvere i problemi di installazione di DKIM

Se si verificano problemi per l'abilitazione di DKIM per il dominio personalizzato, attenersi alla procedura seguente:

- La maggior parte dei problemi di installazione di DKIM è correlata a record DNS non corretti. Verificare che il record CNAME di DKIM (**non** un record TXT) sia formattato correttamente. Per ulteriori informazioni, vedere questo [argomento](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

- Dopo aver creato o aggiornato i record DNS di DKIM nel servizio di hosting DNS per il dominio (in genere, il registrar), attendere che i record DNS vengano propagati.

- Se non è possibile creare i record DNS di DKIM nell'interfaccia di amministrazione, è \<possibile\> sostituire CustomDomain con il dominio personalizzato, ad esempio contoso.com, ed eseguire questo comando in [PowerShell di Exchange Online](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.
