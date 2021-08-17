---
title: Installazione DKIM
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
ms.openlocfilehash: 5dc90965516cc4d360b9be56c7737c6d134123ea8ac263b092559dd1416faff4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54108560"
---
# <a name="setup-dkim"></a>Installazione DKIM

Le istruzioni complete per la configurazione di DKIM per i domini personalizzati in Microsoft 365 [sono disponibili qui.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)

1. Per **ogni** dominio personalizzato, è necessario creare **due** record CNAME DKIM nel servizio di hosting DNS del dominio (in genere, il registrar). Ad esempio, contoso.com e fourthcoffee.com richiedono quattro record CNAME DKIM: due per contoso.com e due per fourthcoffee.com.

   I record CNAME DKIM per **ogni** dominio personalizzato utilizzano i formati seguenti:

   - **Nome host**: `selector1._domainkey.<CustomDomain>`

     **Punta all'indirizzo o al valore**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Nome host**: `selector2._domainkey.<CustomDomain>`

     **Punta all'indirizzo o al valore**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> è il testo a sinistra di nel record MX personalizzato per il dominio personalizzato (ad esempio, per il `.mail.protection.outlook.com` `contoso-com` dominio contoso.com). \<InitialDomain\>è il dominio utilizzato per l'accesso a Microsoft 365 (ad esempio, contoso.onmicrosoft.com).

2. Dopo aver creato i record CNAME per i domini personalizzati, completare le istruzioni seguenti:

   a. [accedi a Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) con il tuo account aziendale o dell'istituto di istruzione.

   b. Selezionare l'icona di avvio delle app in alto a sinistra e scegliere **Amministratore**.

   c. Nel riquadro di spostamento in basso a sinistra, espandere **Amministrazione** e scegliere **Exchange**.

   d. Passare a **Protezione**  >  **DKIM**.

   e. Selezionare il dominio e quindi scegliere **Abilita** per Firmare i messaggi per questo dominio con firme **DKIM**. Ripetere questo passaggio per ogni dominio personalizzato.
