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
ms.openlocfilehash: cb1f621dffc88464c339b55998efb5440cfd775c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332311"
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
**Nota:** **DomainGUID** è il testo a sinistra di **.mail.protection.outlook.com** nel record MX personalizzato per il dominio personalizzato (ad esempio, contoso-com per il dominio **contoso.com**). **InitialDomain** è il dominio utilizzato per l'accesso a Office 365 (ad esempio, **contoso.onmicrosoft.com**).

Per ulteriori informazioni sui record DNS, vedere [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).