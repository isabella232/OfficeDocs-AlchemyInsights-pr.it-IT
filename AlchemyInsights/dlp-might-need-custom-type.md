---
title: DLP potrebbe essere necessario un tipo personalizzato
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 890bba57bc36c034c507e6124cd6593ef4d92af8
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932662"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="0ab2d-102">DLP potrebbe essere necessario un tipo personalizzato</span><span class="sxs-lookup"><span data-stu-id="0ab2d-102">DLP might need a custom type</span></span>

<span data-ttu-id="0ab2d-103">**Importante**: molti clienti di SharePoint Online e OneDrive eseguono applicazioni aziendali critiche rispetto al servizio in esecuzione in background.</span><span class="sxs-lookup"><span data-stu-id="0ab2d-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="0ab2d-104">Tali applicazioni includono soluzioni per la migrazione del contenuto, di Prevenzione della perdita dei dati e per il backup.</span><span class="sxs-lookup"><span data-stu-id="0ab2d-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="0ab2d-105">In questi tempi straordinari, stiamo adottando misure per garantire che i servizi di SharePoint Online e OneDrive rimangano altamente disponibili e affidabili per gli utenti che dipendono ancor più dal servizio negli scenari di lavoro remoto.</span><span class="sxs-lookup"><span data-stu-id="0ab2d-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="0ab2d-106">A sostegno di questo obiettivo, abbiamo implementato limitazioni più rigide sulle app in background (migrazione, prevenzione della perdita dei dati e soluzioni di backup) durante il giorni nei giorni feriali.</span><span class="sxs-lookup"><span data-stu-id="0ab2d-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="0ab2d-107">In questo periodo sarà possibile notare una riduzione della velocità effettiva in queste app.</span><span class="sxs-lookup"><span data-stu-id="0ab2d-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="0ab2d-108">Tuttavia, nelle ore serali e durante il fine settimana nell'area il servizio sarà predisposto per elaborare una quantità notevolmente superiore di richieste delle app in background.</span><span class="sxs-lookup"><span data-stu-id="0ab2d-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="0ab2d-109">**DLP potrebbe richiedere un tipo di informazioni personalizzato**</span><span class="sxs-lookup"><span data-stu-id="0ab2d-109">**DLP may require a custom information type**</span></span>

<span data-ttu-id="0ab2d-110">Con un criterio di prevenzione della perdita di dati (DLP), è possibile identificare e proteggere i dati sensibili nell'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="0ab2d-110">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="0ab2d-111">In alcuni scenari potrebbe essere necessario creare un tipo di informazioni riservate **personalizzato** per proteggere i dati dell'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="0ab2d-111">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="0ab2d-112">Ad esempio, è possibile che l'organizzazione debba identificare e proteggere gli ID dei dipendenti o altri dati in un formato specifico per l'org. In caso affermativo, vedere gli articoli seguenti per ulteriori informazioni.</span><span class="sxs-lookup"><span data-stu-id="0ab2d-112">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="0ab2d-113">**Personalizzare una tipologia integrata di informazioni sensibili**</span><span class="sxs-lookup"><span data-stu-id="0ab2d-113">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="0ab2d-114">Se un tipo di informazioni riservate incorporato soddisfa le proprie esigenze con solo alcuni ritocchi, è possibile [personalizzare un tipo di informazioni riservate incorporato](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="0ab2d-114">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="0ab2d-115">Ad esempio, è possibile aggiungere o rimuovere parole chiave oppure aggiungere o rimuovere elementi di prova di supporto quali una data o un indirizzo.</span><span class="sxs-lookup"><span data-stu-id="0ab2d-115">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="0ab2d-116">**Creare una tipologia personalizzata di informazioni riservate**</span><span class="sxs-lookup"><span data-stu-id="0ab2d-116">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="0ab2d-117">Tuttavia, se è necessario identificare e proteggere complessivamente un tipo diverso di informazioni riservate, è possibile [creare un tipo di informazioni riservate personalizzato](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) nell'interfaccia utente del centro sicurezza & conformità.</span><span class="sxs-lookup"><span data-stu-id="0ab2d-117">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="0ab2d-118">**Creare un tipo di informazioni sensibili personalizzato in PowerShell per Centro sicurezza e conformità**</span><span class="sxs-lookup"><span data-stu-id="0ab2d-118">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="0ab2d-119">Infine, se l'interfaccia utente non fornisce tutte le opzioni necessarie, è possibile [creare un tipo di informazioni riservate personalizzato nel centro sicurezza & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="0ab2d-119">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="0ab2d-120">Se si inizia con un file XML, è possibile utilizzare tutte le opzioni disponibili.</span><span class="sxs-lookup"><span data-stu-id="0ab2d-120">By starting with an XML file, you can use every option available.</span></span>
