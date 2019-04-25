---
title: Regola DLP per il SSN non funzionante
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
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32404421"
---
Se si riscontrano problemi con la **prevenzione della perdita di dati (DLP),** non funziona per i contenuti che contengono un numero di previdenza **sociale (SSN)** quando si utilizza un tipo di informazioni riservate in Office 365? In caso affermativo, verificare che il contenuto contenga le informazioni necessarie per l'aspetto del criterio DLP. 
  
Ad esempio, per i criteri SSN configurati con un livello di confidenza pari al 85%, vengono valutati e devono essere individuati i seguenti per attivare la regola:
  
- **[Formato:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 cifre, che possono essere in un modello formattato o non formattato 
    
- **[Motivo:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Quattro funzioni cercano SNSS in quattro modelli diversi: 
    
  - Func_ssn trova SNSS con una formattazione complessa pre2011 che è formattata con trattini o spazi (ddd-dd-dddd o ddd dd dddd)
    
  - Func_unformatted_ssn trova SNSS con una formattazione complessa pre2011 che non è formattata come nove cifre consecutive (ddddddddd)
    
  - Func_randomized_formatted_ssn trova post-2011 SNSS formattati con trattini o spazi (ddd-dd-dddd o ddd dd dddd)
    
  - Func_randomized_unformatted_ssn trova post-2011 SNSS che non sono formattati come nove cifre consecutive (ddddddddd)
    
- **[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, non c'è nessun checksum 
    
- **[Definizione:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** Un criterio DLP è 85% fiducioso di aver rilevato questo tipo di informazioni riservate se, entro 300 caratteri: 
    
  - La [funzione Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) trova contenuto che corrisponde al modello. 
    
  - Viene trovata una parola chiave da [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn). Tra gli esempi di parole chiave sono inclusi: *Social Security, Social Security #, SOC sec, SSN* . Ad esempio, il seguente esempio verrebbe attivato per il criterio DLP SSN: **SSN: 489-36-8350**
    
Per ulteriori informazioni su ciò che è necessario per rilevare SNSS per il contenuto, vedere la sezione seguente in questo articolo: [che cosa i tipi di informazioni riservate cercano SNSS](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
Se si utilizza un tipo di informazioni riservate predefinito diverso, vedere l'articolo seguente per informazioni su ciò che è necessario per gli altri tipi: [che cosa cercano i tipi di informazioni riservate](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

