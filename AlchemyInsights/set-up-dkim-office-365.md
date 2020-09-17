---
title: Setup DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: b34bfdafcab6229a4dd2e9d9f23103fa13556482
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47808711"
---
# <a name="setup-dkim"></a>Setup DKIM

Di [seguito](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)sono riportate le istruzioni complete per la configurazione di DKIM per i domini personalizzati in Microsoft 365.

1. Per **ogni** dominio personalizzato, è necessario creare **due** record CNAME di DKIM nel servizio di hosting DNS del dominio (in genere, il registrar). Ad esempio, contoso.com e fourthcoffee.com richiedono quattro record CNAME di DKIM: due per contoso.com e due per fourthcoffee.com.

   I record CNAME di DKIM per **ogni** dominio personalizzato utilizzano i formati seguenti:

   - **Nome host**: `selector1._domainkey.<CustomDomain>`

     **Punta all'indirizzo o al valore**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Nome host**: `selector2._domainkey.<CustomDomain>`

     **Punta all'indirizzo o al valore**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> è il testo a sinistra del `.mail.protection.outlook.com` record MX personalizzato per il dominio personalizzato, ad esempio `contoso-com` per il dominio contoso.com. \<InitialDomain\> è il dominio utilizzato per l'accesso a Microsoft 365 (ad esempio, contoso.onmicrosoft.com).

2. Dopo aver creato i record CNAME per i domini personalizzati, completare le seguenti istruzioni:

   a. [accedere a Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) con l'account aziendale o dell'Istituto di istruzione.

   b. Selezionare l'icona di avvio delle app in alto a sinistra e scegliere **Amministratore**.

   c. Nel riquadro di spostamento in basso a sinistra, espandere **Amministrazione** e scegliere **Exchange**.

   d. Andare a **Protection**  >  **DKIM**.

   e. Selezionare il dominio e quindi fare clic su **Abilita** per **i messaggi di firma per questo dominio con firme DKIM**. Ripetere questo passaggio per ogni dominio personalizzato.
