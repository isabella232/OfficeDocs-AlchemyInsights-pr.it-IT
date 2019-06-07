---
title: Setup DKIM in Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 0f81fe02135f3d0901ffe5a26d7aa3dad70c3770
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765187"
---
# <a name="setup-dkim-in-office-365"></a>Setup DKIM in Office 365

Di [seguito](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365)sono riportate le istruzioni complete per la configurazione di DKIM per i domini personalizzati in Office 365.

1. Per **ogni** dominio personalizzato, è necessario creare **due** record CNAME di DKIM nel servizio di hosting DNS del dominio (in genere, il registrar). Ad esempio, contoso.com e fourthcoffee.com richiedono quattro record CNAME di DKIM: due per contoso.com e due per fourthcoffee.com.

   I record CNAME di DKIM per **ogni** dominio personalizzato utilizzano i formati seguenti:

   - **Nome host**:`selector1._domainkey.<CustomDomain>`

     **Punta all'indirizzo o al valore**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Nome host**:`selector2._domainkey.<CustomDomain>`

     **Punta all'indirizzo o al valore**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> è il testo a sinistra del `.mail.protection.outlook.com` record MX personalizzato per il dominio personalizzato, `contoso-com` ad esempio per il dominio contoso.com. \<InitialDomain\> è il dominio utilizzato per l'accesso a Office 365 (ad esempio, contoso.onmicrosoft.com).

2. Dopo aver creato i record CNAME per i domini personalizzati, completare le seguenti istruzioni:

   un. [Accedere a Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) con il proprio account aziendale o dell'istituto di istruzione.

   b. Selezionare l'icona di avvio delle app in alto a sinistra e scegliere **Amministratore**.

   c. Nel riquadro di spostamento in basso a sinistra, espandere **Amministrazione** e scegliere **Exchange**.

   d. Andare a **Protection** > **DKIM**.

   e. Selezionare il dominio e quindi fare clic su **Abilita** per **i messaggi di firma per questo dominio con firme DKIM**. Ripetere questo passaggio per ogni dominio personalizzato.
