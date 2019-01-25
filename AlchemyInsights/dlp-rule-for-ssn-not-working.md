---
title: Regole DLP per SSN non funziona
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: b92d122b774d97cd2e44cc0880dc5001065b57cc
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/24/2019
ms.locfileid: "29476408"
---
Si sono verificati problemi con **Prevenzione della perdita di dati (DLP)** non funziona per il contenuto che include un **Numero di previdenza sociale (SSN)** quando si utilizza un tipo di informazioni riservate in Office 365? In tal caso, verificare che il contenuto sono contenute le informazioni necessarie per quali il criterio DLP è alla ricerca. 
  
Ad esempio, per un criterio SSN configurato con un livello di probabilità di 85%, le operazioni seguenti vengono valutati le proprietà e devono essere rilevati della regola da attivare:
  
- **[Formato:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 cifre, che possono avere un motivo formattato o 
    
- **[Motivo:](https://msconnect.microsoft.com/https:/docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Quattro funzioni cercare SSNs in quattro formati diversi: 
    
  - Func_ssn trova SSNs di pre-2011 sicuro formattazione formattati con trattini o spazi (ggg-gg-gggg OR ggg gg gggg)
    
  - Func_unformatted_ssn trova SSNs di pre-2011 sicuro la formattazione viene formattato come nove cifre consecutive (ddddddddd)
    
  - Func_randomized_formatted_ssn trova SSNs post 2011 formattati con trattini o spazi (ggg-gg-gggg OR ggg gg gggg)
    
  - Func_randomized_unformatted_ssn trova SSNs post 2011 che viene formattato come nove cifre consecutive (ddddddddd)
    
- **[Checksum:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, non esiste alcun Checksum 
    
- **[Definizione:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** Un criterio DLP è 85% la certezza che è stato rilevato questo tipo di informazioni riservate se all'interno di prossimità di 300 caratteri: 
    
  - La funzione Func_ssn restituisce contenuti che corrispondono al modello. 
    
  - È possibile trovare una parola chiave da [Keyword_ssn](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) . Sono inclusi alcuni esempi di parole chiave: *previdenza sociale, previdenza sociale #, Soc Sec, SSN* . Nell'esempio seguente, ad esempio attiverà per il criterio DLP SSN: **SSN: 8350 di 36 489**
    
Per ulteriori informazioni sul funzionamento di SSNs devono essere rilevate per il contenuto, vedere la sezione seguente in questo articolo: [Che cosa the riservati tipi di informazioni cercare SSNs](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
Utilizzo di un tipo di informazioni riservate predefinite diverse, vedere l'articolo seguente per informazioni su cosa è necessario per altri tipi: [cercare cosa the riservati tipi di informazioni](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

