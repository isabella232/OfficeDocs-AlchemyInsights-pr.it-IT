---
title: Regole DLP per Stati Uniti / numero di passaporto Regno Unito non funziona
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 716d1030d93ce006c36d7925fb132e974ae8feb4
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/15/2019
ms.locfileid: "28296946"
---
<span data-ttu-id="62f1d-p101">Si sono verificati problemi con **Prevenzione della perdita di dati (DLP)** non funziona per contenuto contenente un **US / numero di passaporto Regno Unito** quando si utilizza un tipo di informazioni riservate DLP in Office 365? In tal caso, verificare che il contenuto contiene le informazioni necessarie per quali il criterio DLP è cercando quando viene valutata.</span><span class="sxs-lookup"><span data-stu-id="62f1d-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK Passport Number** when using a DLP sensitive information type in O365? If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span> 
  
<span data-ttu-id="62f1d-104">Ad esempio, per un **US / numero di passaporto Regno Unito** criterio configurato con un livello di probabilità pari al 75%, i seguenti vengono valutati le proprietà e devono essere rilevati della regola da attivare</span><span class="sxs-lookup"><span data-stu-id="62f1d-104">For example, for a **US/UK Passport Number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span> 
  
- <span data-ttu-id="62f1d-105">**[Formato:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nove cifre</span><span class="sxs-lookup"><span data-stu-id="62f1d-105">**[Format:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span> 
    
- <span data-ttu-id="62f1d-106">**[Motivo:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nove cifre consecutive</span><span class="sxs-lookup"><span data-stu-id="62f1d-106">**[Pattern:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span> 
    
- <span data-ttu-id="62f1d-107">**[Checksum:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, non esiste alcun Checksum</span><span class="sxs-lookup"><span data-stu-id="62f1d-107">**[Checksum:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="62f1d-108">**[Definizione:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** Un criterio DLP è 75% la certezza che è stato rilevato questo tipo di informazioni riservate se all'interno di prossimità di 300 caratteri:</span><span class="sxs-lookup"><span data-stu-id="62f1d-108">**[Definition:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="62f1d-109">La funzione Func_usa_uk_passport restituisce contenuti che corrispondono al modello.</span><span class="sxs-lookup"><span data-stu-id="62f1d-109">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>
    
  - <span data-ttu-id="62f1d-110">Viene trovata una parola chiave da Keyword_passport.</span><span class="sxs-lookup"><span data-stu-id="62f1d-110">A keyword from Keyword_passport is found.</span></span>
    
    <span data-ttu-id="62f1d-111">Attiverà, ad esempio, nell'esempio seguente per il **US / numero di passaporto Regno Unito** criteri: numero di passaporto 123456789</span><span class="sxs-lookup"><span data-stu-id="62f1d-111">For example, the following sample would trigger for the **US/UK Passport Number** policy: U.S. Passport number 123456789</span></span> 
    
<span data-ttu-id="62f1d-112">Per ulteriori informazioni sul funzionamento di un attributo inglese Americano / numero di passaporto Regno Unito devono essere rilevate per il contenuto, vedere la sezione seguente in questo articolo: [interfaccia cosa the riservati tipi di informazioni per Stati Uniti / numero di passaporto Regno Unito](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="62f1d-112">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="62f1d-113">Utilizzo di un tipo di informazioni riservate predefinite diverse, vedere l'articolo seguente per informazioni su cosa è necessario per altri tipi: [cercare cosa the riservati tipi di informazioni](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="62f1d-113">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

