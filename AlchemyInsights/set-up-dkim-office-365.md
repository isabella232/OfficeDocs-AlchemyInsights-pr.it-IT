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
# <a name="setup-dkim"></a><span data-ttu-id="ce673-102">Setup DKIM</span><span class="sxs-lookup"><span data-stu-id="ce673-102">Setup DKIM</span></span>

<span data-ttu-id="ce673-103">Di [seguito](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)sono riportate le istruzioni complete per la configurazione di DKIM per i domini personalizzati in Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="ce673-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

1. <span data-ttu-id="ce673-104">Per **ogni** dominio personalizzato, è necessario creare **due** record CNAME di DKIM nel servizio di hosting DNS del dominio (in genere, il registrar).</span><span class="sxs-lookup"><span data-stu-id="ce673-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="ce673-105">Ad esempio, contoso.com e fourthcoffee.com richiedono quattro record CNAME di DKIM: due per contoso.com e due per fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="ce673-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="ce673-106">I record CNAME di DKIM per **ogni** dominio personalizzato utilizzano i formati seguenti:</span><span class="sxs-lookup"><span data-stu-id="ce673-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="ce673-107">**Nome host**: `selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="ce673-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="ce673-108">**Punta all'indirizzo o al valore**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="ce673-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="ce673-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="ce673-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="ce673-110">**Nome host**: `selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="ce673-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="ce673-111">**Punta all'indirizzo o al valore**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="ce673-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="ce673-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="ce673-112">**TTL**: 3600</span></span>

   <span data-ttu-id="ce673-113">\<DomainGUID\> è il testo a sinistra del `.mail.protection.outlook.com` record MX personalizzato per il dominio personalizzato, ad esempio `contoso-com` per il dominio contoso.com.</span><span class="sxs-lookup"><span data-stu-id="ce673-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="ce673-114">\<InitialDomain\> è il dominio utilizzato per l'accesso a Microsoft 365 (ad esempio, contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="ce673-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="ce673-115">Dopo aver creato i record CNAME per i domini personalizzati, completare le seguenti istruzioni:</span><span class="sxs-lookup"><span data-stu-id="ce673-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="ce673-116">a.</span><span class="sxs-lookup"><span data-stu-id="ce673-116">a.</span></span> <span data-ttu-id="ce673-117">[accedere a Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) con l'account aziendale o dell'Istituto di istruzione.</span><span class="sxs-lookup"><span data-stu-id="ce673-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="ce673-118">b.</span><span class="sxs-lookup"><span data-stu-id="ce673-118">b.</span></span> <span data-ttu-id="ce673-119">Selezionare l'icona di avvio delle app in alto a sinistra e scegliere **Amministratore**.</span><span class="sxs-lookup"><span data-stu-id="ce673-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="ce673-120">c.</span><span class="sxs-lookup"><span data-stu-id="ce673-120">c.</span></span> <span data-ttu-id="ce673-121">Nel riquadro di spostamento in basso a sinistra, espandere **Amministrazione** e scegliere **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="ce673-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="ce673-122">d.</span><span class="sxs-lookup"><span data-stu-id="ce673-122">d.</span></span> <span data-ttu-id="ce673-123">Andare a **Protection**  >  **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="ce673-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="ce673-124">e.</span><span class="sxs-lookup"><span data-stu-id="ce673-124">e.</span></span> <span data-ttu-id="ce673-125">Selezionare il dominio e quindi fare clic su **Abilita** per **i messaggi di firma per questo dominio con firme DKIM**.</span><span class="sxs-lookup"><span data-stu-id="ce673-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="ce673-126">Ripetere questo passaggio per ogni dominio personalizzato.</span><span class="sxs-lookup"><span data-stu-id="ce673-126">Repeat this step for each custom domain.</span></span>
