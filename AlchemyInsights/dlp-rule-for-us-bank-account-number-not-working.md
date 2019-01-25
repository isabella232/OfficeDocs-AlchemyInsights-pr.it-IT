---
title: Regole DLP per noi numero di conto bancario non funziona
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 6eae9146d33f5fc307085dbf931d57bdbb28b82e
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/24/2019
ms.locfileid: "29475510"
---
<span data-ttu-id="58adf-p101">Si sono verificati problemi con **Prevenzione della perdita di dati (DLP)** non funziona per il contenuto che include un **Numero di conto bancario US** quando si utilizza un tipo di informazioni riservate DLP in Office 365? In tal caso, verificare che il contenuto contiene le informazioni necessarie per quali il criterio DLP è cercando quando viene valutata.</span><span class="sxs-lookup"><span data-stu-id="58adf-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365? If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span> 
  
<span data-ttu-id="58adf-104">Ad esempio, per un criterio di **Numero di conto bancario US** configurato con un livello di probabilità di 85%, le operazioni seguenti vengono valutati le proprietà e devono essere rilevati della regola da attivare:</span><span class="sxs-lookup"><span data-stu-id="58adf-104">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span> 
  
- <span data-ttu-id="58adf-105">**[Formato:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 17 8 cifre</span><span class="sxs-lookup"><span data-stu-id="58adf-105">**[Format:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digits</span></span> 
    
- <span data-ttu-id="58adf-106">**[Motivo:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 17 8 cifre consecutive.</span><span class="sxs-lookup"><span data-stu-id="58adf-106">**[Pattern:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 consecutive digits.</span></span> 
    
- <span data-ttu-id="58adf-107">**[Checksum:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, non esiste alcun Checksum</span><span class="sxs-lookup"><span data-stu-id="58adf-107">**[Checksum:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="58adf-108">**[Definizione:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)** Un criterio DLP è 75% la certezza che è stato rilevato questo tipo di informazioni riservate se all'interno di prossimità di 300 caratteri:</span><span class="sxs-lookup"><span data-stu-id="58adf-108">**[Definition:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="58adf-109">L'espressione regolare Regex_usa_bank_account_number restituisce contenuti che corrispondono al modello.</span><span class="sxs-lookup"><span data-stu-id="58adf-109">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>
    
  - <span data-ttu-id="58adf-110">Viene trovata una parola chiave da Keyword_usa_Bank_Account.</span><span class="sxs-lookup"><span data-stu-id="58adf-110">A keyword from Keyword_usa_Bank_Account is found.</span></span>
    
    <span data-ttu-id="58adf-111">Nell'esempio seguente, ad esempio attiverà per il criterio di **Numero di conto bancario negli Stati Uniti** : 78344011 conto corrente</span><span class="sxs-lookup"><span data-stu-id="58adf-111">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span> 
    
<span data-ttu-id="58adf-112">Per ulteriori informazioni sul funzionamento di un **Numero di conto bancario negli Stati Uniti** e rilevato per il contenuto, vedere la sezione seguente in questo articolo: [Che cosa the riservati tipi di informazioni cercare il numero di conto bancario negli Stati Uniti](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="58adf-112">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span></span>
  
<span data-ttu-id="58adf-113">Utilizzo di un tipo di informazioni riservate predefinite diverse, vedere l'articolo seguente per informazioni su cosa è necessario per altri tipi: [cercare cosa the riservati tipi di informazioni](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="58adf-113">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

