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
Se si riscontrano problemi con la **prevenzione della perdita di dati (DLP),** non funziona per il contenuto contenente un **numero di carta di credito** quando si utilizza un tipo di informazioni riservate DLP in O365? In caso affermativo, verificare che il contenuto contenga le informazioni necessarie per attivare il criterio DLP quando viene valutato. Ad esempio, per i **criteri delle carte di credito** configurati con un livello di confidenza pari al 85%, vengono valutati e devono essere rilevati i seguenti elementi per attivare la regola: 
  
- **[Formato:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 cifre che possono essere formattate o non formattate (dddddddddddddddd) e devono superare il test di Luhn. 
    
- **[Motivo:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Modello molto complesso e robusto che rileva le schede di tutte le principali marche di tutto il mondo, tra cui Visa, MasterCard, Discover Card, JCB, American Express, Gift Cards e Diner Cards. 
    
- **[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Sì, il checksum di Luhn 
    
- **[Definizione:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Un criterio DLP è 85% fiducioso di aver rilevato questo tipo di informazioni riservate se, entro 300 caratteri: 
    
  - La funzione Func_credit_card restituisce contenuti che corrispondono al modello.
    
  - Si verifica una delle situazioni seguenti: 
    
  - Viene trovata una parola chiave da Keyword_cc_verification.
    
  - Viene trovata una parola chiave da Keyword_cc_name
    
  - La funzione Func_expiration_date rileva una data nel formato corretto.
    
  - Il checksum passa
    
    Ad esempio, il seguente esempio si innescherà per un criterio di numero di carta di credito DLP:
    
  - Visa: 4485 3647 3952 7352 
    
  - Scade: 2/2009
    
Per ulteriori informazioni su ciò che è necessario affinché venga rilevato un **numero di carta di credito** per il contenuto, vedere la sezione seguente di questo articolo: informazioni sui [tipi di informazione sensibili ricerca per la carta di credito](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number) .
  
Se si utilizza un tipo di informazioni riservate predefinito diverso, vedere l'articolo seguente per informazioni su ciò che è necessario per gli altri tipi: [che cosa cercano i tipi di informazioni riservate](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

