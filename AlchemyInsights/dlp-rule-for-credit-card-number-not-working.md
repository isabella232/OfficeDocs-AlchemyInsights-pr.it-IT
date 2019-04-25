---
title: Regola DLP per il numero di carta di credito non funzionante
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
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32404506"
---
<span data-ttu-id="6f826-102">Se si riscontrano problemi con la **prevenzione della perdita di dati (DLP),** non funziona per il contenuto contenente un **numero di carta di credito** quando si utilizza un tipo di informazioni riservate DLP in O365?</span><span class="sxs-lookup"><span data-stu-id="6f826-102">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="6f826-103">In caso affermativo, verificare che il contenuto contenga le informazioni necessarie per attivare il criterio DLP quando viene valutato.</span><span class="sxs-lookup"><span data-stu-id="6f826-103">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="6f826-104">Ad esempio, per i **criteri delle carte di credito** configurati con un livello di confidenza pari al 85%, vengono valutati e devono essere rilevati i seguenti elementi per attivare la regola:</span><span class="sxs-lookup"><span data-stu-id="6f826-104">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span> 
  
- <span data-ttu-id="6f826-105">**[Formato:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 cifre che possono essere formattate o non formattate (dddddddddddddddd) e devono superare il test di Luhn.</span><span class="sxs-lookup"><span data-stu-id="6f826-105">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span> 
    
- <span data-ttu-id="6f826-106">**[Motivo:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Modello molto complesso e robusto che rileva le schede di tutte le principali marche di tutto il mondo, tra cui Visa, MasterCard, Discover Card, JCB, American Express, Gift Cards e Diner Cards.</span><span class="sxs-lookup"><span data-stu-id="6f826-106">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span> 
    
- <span data-ttu-id="6f826-107">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Sì, il checksum di Luhn</span><span class="sxs-lookup"><span data-stu-id="6f826-107">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span> 
    
- <span data-ttu-id="6f826-108">**[Definizione:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Un criterio DLP è 85% fiducioso di aver rilevato questo tipo di informazioni riservate se, entro 300 caratteri:</span><span class="sxs-lookup"><span data-stu-id="6f826-108">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="6f826-109">La funzione Func_credit_card restituisce contenuti che corrispondono al modello.</span><span class="sxs-lookup"><span data-stu-id="6f826-109">The function Func_credit_card finds content that matches the pattern.</span></span>
    
  - <span data-ttu-id="6f826-110">Si verifica una delle situazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="6f826-110">One of the following is true:</span></span> 
    
  - <span data-ttu-id="6f826-111">Viene trovata una parola chiave da Keyword_cc_verification.</span><span class="sxs-lookup"><span data-stu-id="6f826-111">A keyword from Keyword_cc_verification is found.</span></span>
    
  - <span data-ttu-id="6f826-112">Viene trovata una parola chiave da Keyword_cc_name</span><span class="sxs-lookup"><span data-stu-id="6f826-112">A keyword from Keyword_cc_name is found</span></span>
    
  - <span data-ttu-id="6f826-113">La funzione Func_expiration_date rileva una data nel formato corretto.</span><span class="sxs-lookup"><span data-stu-id="6f826-113">The function Func_expiration_date finds a date in the right date format.</span></span>
    
  - <span data-ttu-id="6f826-114">Il checksum passa</span><span class="sxs-lookup"><span data-stu-id="6f826-114">The checksum passes</span></span>
    
    <span data-ttu-id="6f826-115">Ad esempio, il seguente esempio si innescherà per un criterio di numero di carta di credito DLP:</span><span class="sxs-lookup"><span data-stu-id="6f826-115">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>
    
  - <span data-ttu-id="6f826-116">Visa: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="6f826-116">Visa: 4485 3647 3952 7352</span></span> 
    
  - <span data-ttu-id="6f826-117">Scade: 2/2009</span><span class="sxs-lookup"><span data-stu-id="6f826-117">Expires: 2/2009</span></span>
    
<span data-ttu-id="6f826-118">Per ulteriori informazioni su ciò che è necessario affinché venga rilevato un **numero di carta di credito** per il contenuto, vedere la sezione seguente di questo articolo: informazioni sui [tipi di informazione sensibili ricerca per la carta di credito](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number) .</span><span class="sxs-lookup"><span data-stu-id="6f826-118">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="6f826-119">Se si utilizza un tipo di informazioni riservate predefinito diverso, vedere l'articolo seguente per informazioni su ciò che è necessario per gli altri tipi: [che cosa cercano i tipi di informazioni riservate](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="6f826-119">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

