---
title: Setup DKIM in Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: dd908db6a4bc1739b3c1cff059387034d67e093d
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666268"
---
# <a name="setup-dkim-in-office-365"></a><span data-ttu-id="bd65c-102">Setup DKIM in Office 365</span><span class="sxs-lookup"><span data-stu-id="bd65c-102">Setup DKIM in Office 365</span></span>

<span data-ttu-id="bd65c-103">Di [seguito](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365)sono riportate le istruzioni complete per la configurazione di DKIM per i domini personalizzati in Office 365.</span><span class="sxs-lookup"><span data-stu-id="bd65c-103">The complete instructions for configuring DKIM for custom domains in Office 365 are [here](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

1. <span data-ttu-id="bd65c-104">Per **ogni** dominio personalizzato, è necessario creare **due** record CNAME di DKIM nel servizio di hosting DNS del dominio (in genere, il registrar).</span><span class="sxs-lookup"><span data-stu-id="bd65c-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="bd65c-105">Ad esempio, contoso.com e fourthcoffee.com richiedono quattro record CNAME di DKIM: due per contoso.com e due per fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="bd65c-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="bd65c-106">I record CNAME di DKIM per **ogni** dominio personalizzato utilizzano i formati seguenti:</span><span class="sxs-lookup"><span data-stu-id="bd65c-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="bd65c-107">**Nome host**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="bd65c-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="bd65c-108">**Punta all'indirizzo o al valore**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="bd65c-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="bd65c-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="bd65c-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="bd65c-110">**Nome host**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="bd65c-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="bd65c-111">**Punta all'indirizzo o al valore**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="bd65c-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="bd65c-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="bd65c-112">**TTL**: 3600</span></span>

   <span data-ttu-id="bd65c-113">\<DomainGUID\> è il testo a sinistra del `.mail.protection.outlook.com` record MX personalizzato per il dominio personalizzato, `contoso-com` ad esempio per il dominio contoso.com.</span><span class="sxs-lookup"><span data-stu-id="bd65c-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="bd65c-114">\<InitialDomain\> è il dominio utilizzato per l'accesso a Office 365 (ad esempio, contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="bd65c-114">\<InitialDomain\> is the domain you used when you signed up for Office 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="bd65c-115">Dopo aver creato i record CNAME per i domini personalizzati, completare le seguenti istruzioni:</span><span class="sxs-lookup"><span data-stu-id="bd65c-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="bd65c-116">un.</span><span class="sxs-lookup"><span data-stu-id="bd65c-116">a.</span></span> <span data-ttu-id="bd65c-117">[Accedere a Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) con il proprio account aziendale o dell'istituto di istruzione.</span><span class="sxs-lookup"><span data-stu-id="bd65c-117">[Sign in to Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="bd65c-118">b.</span><span class="sxs-lookup"><span data-stu-id="bd65c-118">b.</span></span> <span data-ttu-id="bd65c-119">Selezionare l'icona di avvio delle app in alto a sinistra e scegliere **Amministratore**.</span><span class="sxs-lookup"><span data-stu-id="bd65c-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="bd65c-120">c.</span><span class="sxs-lookup"><span data-stu-id="bd65c-120">c.</span></span> <span data-ttu-id="bd65c-121">Nel riquadro di spostamento in basso a sinistra, espandere **Amministrazione** e scegliere **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="bd65c-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="bd65c-122">d.</span><span class="sxs-lookup"><span data-stu-id="bd65c-122">d.</span></span> <span data-ttu-id="bd65c-123">Andare a **Protection** > **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="bd65c-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="bd65c-124">e.</span><span class="sxs-lookup"><span data-stu-id="bd65c-124">e.</span></span> <span data-ttu-id="bd65c-125">Selezionare il dominio e quindi fare clic su **Abilita** per **i messaggi di firma per questo dominio con firme DKIM**.</span><span class="sxs-lookup"><span data-stu-id="bd65c-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="bd65c-126">Ripetere questo passaggio per ogni dominio personalizzato.</span><span class="sxs-lookup"><span data-stu-id="bd65c-126">Repeat this step for each custom domain.</span></span>
