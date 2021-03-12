---
title: Configurare DKIM con domini personalizzati
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/22/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: c448956f0dad0738f4de7507ec4686c738a90a55
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736344"
---
# <a name="set-up-dkim-with-custom-domains"></a>Configurare DKIM con domini personalizzati

È necessario pubblicare due record CNAME per ogni dominio personalizzato in DNS. A tale scopo, utilizzare il formato seguente:

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
> [!NOTE]
> **DomainGUID** è il testo a sinistra di **.mail.protection.outlook.com** nel record MX personalizzato per il dominio personalizzato (ad esempio, contoso-com per il dominio **contoso.com**). **InitialDomain** è il dominio usato per l'accesso a Office 365 (ad esempio, **contoso.onmicrosoft.com**).

Per ulteriori informazioni sui record DNS, vedere [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).