---
title: Regole DLP per numero di carta di credito non funziona
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: e1d60c493a27efb7f724d57051e21fad5bd0242f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29919084"
---
<span data-ttu-id="fa674-p101">Si sono verificati problemi con **Prevenzione della perdita di dati (DLP)** non funziona per il contenuto che include un **Numero di carta di credito** quando si utilizza un tipo di informazioni riservate DLP in Office 365? In tal caso, verificare che il contenuto sono contenute le informazioni necessarie per attivare l'il criterio DLP quando viene valutata. Ad esempio, per un **criterio di carta di credito** configurato con un livello di probabilità di 85%, le operazioni seguenti vengono valutati le proprietà e devono essere rilevati della regola da attivare:</span><span class="sxs-lookup"><span data-stu-id="fa674-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365? If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated. For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span> 
  
- <span data-ttu-id="fa674-105">**[Formato:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 cifre che possono essere formattate o non formattato (dddddddddddddddd) e deve superare la verifica Luhn.</span><span class="sxs-lookup"><span data-stu-id="fa674-105">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span> 
    
- <span data-ttu-id="fa674-106">**[Motivo:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Motivo molto complessa e affidabile che consente di rilevare le schede da tutti i principali marchi tutto il mondo, inclusi Visa, Mastercard, individuare scheda, JCB, American Express, gift card e schede diner.</span><span class="sxs-lookup"><span data-stu-id="fa674-106">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span> 
    
- <span data-ttu-id="fa674-107">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Sì, checksum Luhn</span><span class="sxs-lookup"><span data-stu-id="fa674-107">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span> 
    
- <span data-ttu-id="fa674-108">**[Definizione:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Un criterio DLP è 85% la certezza che è stato rilevato questo tipo di informazioni riservate se all'interno di prossimità di 300 caratteri:</span><span class="sxs-lookup"><span data-stu-id="fa674-108">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="fa674-109">La funzione Func_credit_card restituisce contenuti che corrispondono al modello.</span><span class="sxs-lookup"><span data-stu-id="fa674-109">The function Func_credit_card finds content that matches the pattern.</span></span>
    
  - <span data-ttu-id="fa674-110">Si verifica una delle situazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="fa674-110">One of the following is true:</span></span> 
    
  - <span data-ttu-id="fa674-111">Viene trovata una parola chiave da Keyword_cc_verification.</span><span class="sxs-lookup"><span data-stu-id="fa674-111">A keyword from Keyword_cc_verification is found.</span></span>
    
  - <span data-ttu-id="fa674-112">Viene trovata una parola chiave da Keyword_cc_name</span><span class="sxs-lookup"><span data-stu-id="fa674-112">A keyword from Keyword_cc_name is found</span></span>
    
  - <span data-ttu-id="fa674-113">La funzione Func_expiration_date rileva una data nel formato corretto.</span><span class="sxs-lookup"><span data-stu-id="fa674-113">The function Func_expiration_date finds a date in the right date format.</span></span>
    
  - <span data-ttu-id="fa674-114">Passa il valore di checksum</span><span class="sxs-lookup"><span data-stu-id="fa674-114">The checksum passes</span></span>
    
    <span data-ttu-id="fa674-115">Nell'esempio seguente, ad esempio attiverà per un criterio di numero di carta di credito DLP:</span><span class="sxs-lookup"><span data-stu-id="fa674-115">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>
    
  - <span data-ttu-id="fa674-116">Visa: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="fa674-116">Visa: 4485 3647 3952 7352</span></span> 
    
  - <span data-ttu-id="fa674-117">Scadenza: 2/2009</span><span class="sxs-lookup"><span data-stu-id="fa674-117">Expires: 2/2009</span></span>
    
<span data-ttu-id="fa674-118">Per ulteriori informazioni sul funzionamento di un **Numero di carta di credito** devono essere rilevate per il contenuto, vedere la sezione seguente in questo articolo: [Che cosa the riservati tipi di informazioni cercare carta di credito #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="fa674-118">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="fa674-119">Utilizzo di un tipo di informazioni riservate predefinite diverse, vedere l'articolo seguente per informazioni su cosa è necessario per altri tipi: [cercare cosa the riservati tipi di informazioni](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="fa674-119">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

