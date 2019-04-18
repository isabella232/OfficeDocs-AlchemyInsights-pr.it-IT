---
title: DLP potrebbe essere necessario un tipo personalizzato
ms.author: stephow
author: stephow-MSFT
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: cd5bac5efe3a16d32f9b695c8cb452a1eaa3a796
ms.sourcegitcommit: e87b3f691444db3b9f460c9a3109146dc7ad4f80
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2019
ms.locfileid: "31872388"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="0f982-102">DLP potrebbe essere necessario un tipo personalizzato</span><span class="sxs-lookup"><span data-stu-id="0f982-102">DLP might need a custom type</span></span>

<span data-ttu-id="0f982-103">Con un criterio di prevenzione della perdita di dati (DLP), è possibile identificare e proteggere i dati sensibili nell'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="0f982-103">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="0f982-104">In alcuni scenari potrebbe essere necessario creare un tipo di informazioni riservate **personalizzato** per proteggere i dati dell'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="0f982-104">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="0f982-105">Ad esempio, è possibile che l'organizzazione debba identificare e proteggere gli ID dei dipendenti o altri dati in un formato specifico per l'org. In caso affermativo, vedere gli articoli seguenti per ulteriori informazioni.</span><span class="sxs-lookup"><span data-stu-id="0f982-105">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span> 
  
 <span data-ttu-id="0f982-106">**Personalizzare una tipologia integrata di informazioni sensibili**</span><span class="sxs-lookup"><span data-stu-id="0f982-106">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="0f982-107">Se un tipo di informazioni riservate incorporato soddisfa le proprie esigenze con solo alcuni ritocchi, è possibile [personalizzare un tipo di informazioni riservate incorporato](https://docs.microsoft.com/en-us/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="0f982-107">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/en-us/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="0f982-108">Ad esempio, è possibile aggiungere o rimuovere parole chiave oppure aggiungere o rimuovere elementi di prova di supporto quali una data o un indirizzo.</span><span class="sxs-lookup"><span data-stu-id="0f982-108">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="0f982-109">**Creare un tipo di informazioni sensibili personalizzato**</span><span class="sxs-lookup"><span data-stu-id="0f982-109">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="0f982-110">Tuttavia, se è necessario identificare e proteggere completamente un tipo diverso di informazioni riservate, è possibile [creare un tipo di informazioni riservate personalizzato](https://docs.microsoft.com/en-us/office365/securitycompliance/create-a-custom-sensitive-information-type) nell'interfaccia utente del Centro sicurezza & Compliance.</span><span class="sxs-lookup"><span data-stu-id="0f982-110">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/en-us/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span> 
  
<span data-ttu-id="0f982-111">**Creare un tipo di informazioni riservate personalizzato in PowerShell centro conformità di & di sicurezza**</span><span class="sxs-lookup"><span data-stu-id="0f982-111">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="0f982-112">Infine, se l'interfaccia utente non fornisce tutte le opzioni necessarie, è possibile [creare un tipo di informazioni riservate personalizzato in PowerShell per Centro sicurezza _AMP_ Compliance](https://docs.microsoft.com/en-us/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="0f982-112">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/en-us/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="0f982-113">Se si inizia con un file XML, è possibile utilizzare tutte le opzioni disponibili.</span><span class="sxs-lookup"><span data-stu-id="0f982-113">By starting with an XML file, you can use every option available.</span></span>

    