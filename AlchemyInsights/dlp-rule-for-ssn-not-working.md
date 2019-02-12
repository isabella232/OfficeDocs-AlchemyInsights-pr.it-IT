---
title: Regole DLP per SSN non funziona
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: d2d21fb5546d36990d69b76e3ceb72ce2edf3d80
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29933484"
---
<span data-ttu-id="2233d-p101">Si sono verificati problemi con **Prevenzione della perdita di dati (DLP)** non funziona per il contenuto che include un **Numero di previdenza sociale (SSN)** quando si utilizza un tipo di informazioni riservate in Office 365? In tal caso, verificare che il contenuto sono contenute le informazioni necessarie per quali il criterio DLP è alla ricerca.</span><span class="sxs-lookup"><span data-stu-id="2233d-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365? If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="2233d-104">Ad esempio, per un criterio SSN configurato con un livello di probabilità di 85%, le operazioni seguenti vengono valutati le proprietà e devono essere rilevati della regola da attivare:</span><span class="sxs-lookup"><span data-stu-id="2233d-104">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="2233d-105">**[Formato:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 cifre, che possono avere un motivo formattato o</span><span class="sxs-lookup"><span data-stu-id="2233d-105">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span> 
    
- <span data-ttu-id="2233d-106">**[Motivo:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Quattro funzioni cercare SSNs in quattro formati diversi:</span><span class="sxs-lookup"><span data-stu-id="2233d-106">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span> 
    
  - <span data-ttu-id="2233d-107">Func_ssn trova SSNs di pre-2011 sicuro formattazione formattati con trattini o spazi (ggg-gg-gggg OR ggg gg gggg)</span><span class="sxs-lookup"><span data-stu-id="2233d-107">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>
    
  - <span data-ttu-id="2233d-108">Func_unformatted_ssn trova SSNs di pre-2011 sicuro la formattazione viene formattato come nove cifre consecutive (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="2233d-108">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>
    
  - <span data-ttu-id="2233d-109">Func_randomized_formatted_ssn trova SSNs post 2011 formattati con trattini o spazi (ggg-gg-gggg OR ggg gg gggg)</span><span class="sxs-lookup"><span data-stu-id="2233d-109">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>
    
  - <span data-ttu-id="2233d-110">Func_randomized_unformatted_ssn trova SSNs post 2011 che viene formattato come nove cifre consecutive (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="2233d-110">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>
    
- <span data-ttu-id="2233d-111">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, non esiste alcun Checksum</span><span class="sxs-lookup"><span data-stu-id="2233d-111">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="2233d-112">**[Definizione:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** Un criterio DLP è 85% la certezza che è stato rilevato questo tipo di informazioni riservate se all'interno di prossimità di 300 caratteri:</span><span class="sxs-lookup"><span data-stu-id="2233d-112">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="2233d-113">La [funzione Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) consente di trovare contenuto corrispondente al formato.</span><span class="sxs-lookup"><span data-stu-id="2233d-113">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span> 
    
  - <span data-ttu-id="2233d-p102">È possibile trovare una parola chiave da [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) . Sono inclusi alcuni esempi di parole chiave: *previdenza sociale, previdenza sociale #, Soc Sec, SSN* . Nell'esempio seguente, ad esempio attiverà per il criterio DLP SSN: **SSN: 8350 di 36 489**</span><span class="sxs-lookup"><span data-stu-id="2233d-p102">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found. Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  . For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
    
<span data-ttu-id="2233d-117">Per ulteriori informazioni sul funzionamento di SSNs devono essere rilevate per il contenuto, vedere la sezione seguente in questo articolo: [Che cosa the riservati tipi di informazioni cercare SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="2233d-117">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="2233d-118">Utilizzo di un tipo di informazioni riservate predefinite diverse, vedere l'articolo seguente per informazioni su cosa è necessario per altri tipi: [cercare cosa the riservati tipi di informazioni](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="2233d-118">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

