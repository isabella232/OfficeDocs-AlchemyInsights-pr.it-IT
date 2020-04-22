---
title: DLP potrebbe essere necessario un tipo personalizzato
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: b83bb77383e2ae7e78c31f35c972182c54487c60
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704493"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="ae128-102">DLP potrebbe essere necessario un tipo personalizzato</span><span class="sxs-lookup"><span data-stu-id="ae128-102">DLP might need a custom type</span></span>

<span data-ttu-id="ae128-103">**Importante**: durante questi periodi senza precedenti, stiamo adottando misure per garantire che i servizi SharePoint Online e OneDrive rimangano disponibili. Per altre informazioni, vedere [Modifiche temporanee delle funzionalità di SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="ae128-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="ae128-104">**DLP potrebbe richiedere un tipo di informazioni personalizzato**</span><span class="sxs-lookup"><span data-stu-id="ae128-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="ae128-105">Con un criterio di prevenzione della perdita di dati (DLP), è possibile identificare e proteggere i dati sensibili nell'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="ae128-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="ae128-106">In alcuni scenari potrebbe essere necessario creare un tipo di informazioni riservate **personalizzato** per proteggere i dati dell'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="ae128-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="ae128-107">Ad esempio, è possibile che l'organizzazione debba identificare e proteggere gli ID dei dipendenti o altri dati in un formato specifico per l'org. In caso affermativo, vedere gli articoli seguenti per ulteriori informazioni.</span><span class="sxs-lookup"><span data-stu-id="ae128-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="ae128-108">**Personalizzare una tipologia integrata di informazioni sensibili**</span><span class="sxs-lookup"><span data-stu-id="ae128-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="ae128-109">Se un tipo di informazioni riservate incorporato soddisfa le proprie esigenze con solo alcuni ritocchi, è possibile [personalizzare un tipo di informazioni riservate incorporato](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="ae128-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="ae128-110">Ad esempio, è possibile aggiungere o rimuovere parole chiave oppure aggiungere o rimuovere elementi di prova di supporto quali una data o un indirizzo.</span><span class="sxs-lookup"><span data-stu-id="ae128-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="ae128-111">**Creare una tipologia personalizzata di informazioni riservate**</span><span class="sxs-lookup"><span data-stu-id="ae128-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="ae128-112">Tuttavia, se è necessario identificare e proteggere complessivamente un tipo diverso di informazioni riservate, è possibile [creare un tipo di informazioni riservate personalizzato](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) nell'interfaccia utente del centro sicurezza & conformità.</span><span class="sxs-lookup"><span data-stu-id="ae128-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="ae128-113">**Creare un tipo di informazioni sensibili personalizzato in PowerShell per Centro sicurezza e conformità**</span><span class="sxs-lookup"><span data-stu-id="ae128-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="ae128-114">Infine, se l'interfaccia utente non fornisce tutte le opzioni necessarie, è possibile [creare un tipo di informazioni riservate personalizzato nel centro sicurezza & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="ae128-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="ae128-115">Se si inizia con un file XML, è possibile utilizzare tutte le opzioni disponibili.</span><span class="sxs-lookup"><span data-stu-id="ae128-115">By starting with an XML file, you can use every option available.</span></span>
