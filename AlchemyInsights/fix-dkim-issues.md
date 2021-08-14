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
ms.openlocfilehash: 5a613321ed79e657350ec4d19b1f07ac0a091b227a8268c793a10edd9990d41f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53945935"
---
# <a name="fix-dkim-setup-issues"></a>Risolvere i problemi di installazione di DKIM

Se si verificano problemi durante l'abilitazione di DKIM per il dominio personalizzato, eseguire la procedura seguente:

- La maggior parte dei problemi di configurazione di DKIM è correlata a record DNS non corretti. Verificare che il record CNAME DKIM (**non** un record TXT) sia formattato correttamente. Per ulteriori informazioni, vedere questo [argomento.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)

- Dopo aver creato o aggiornato i record DNS DKIM nel servizio di hosting DNS per il dominio (in genere, il registrar), attendere la propagazione dei record DNS.

- Se non è possibile creare i record DNS DKIM nell'interfaccia di amministrazione, è possibile sostituire con il dominio personalizzato (ad esempio, contoso.com) ed eseguire questo comando \<CustomDomain\> in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
