---
title: Regole DLP per numero di carta di credito non funziona
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 4b8897c5cc8286bc4bd49860658a5a94ad17380d
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/30/2019
ms.locfileid: "29657471"
---
Si sono verificati problemi con **Prevenzione della perdita di dati (DLP)** non funziona per il contenuto che include un **Numero di carta di credito** quando si utilizza un tipo di informazioni riservate DLP in Office 365? In tal caso, verificare che il contenuto sono contenute le informazioni necessarie per attivare l'il criterio DLP quando viene valutata. Ad esempio, per un **criterio di carta di credito** configurato con un livello di probabilità di 85%, le operazioni seguenti vengono valutati le proprietà e devono essere rilevati della regola da attivare: 
  
- **[Formato:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 cifre che possono essere formattate o non formattato (dddddddddddddddd) e deve superare la verifica Luhn. 
    
- **[Motivo:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Motivo molto complessa e affidabile che consente di rilevare le schede da tutti i principali marchi tutto il mondo, inclusi Visa, Mastercard, individuare scheda, JCB, American Express, gift card e schede diner. 
    
- **[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Sì, checksum Luhn 
    
- **[Definizione:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Un criterio DLP è 85% la certezza che è stato rilevato questo tipo di informazioni riservate se all'interno di prossimità di 300 caratteri: 
    
  - La funzione Func_credit_card restituisce contenuti che corrispondono al modello.
    
  - Si verifica una delle situazioni seguenti: 
    
  - Viene trovata una parola chiave da Keyword_cc_verification.
    
  - Viene trovata una parola chiave da Keyword_cc_name
    
  - La funzione Func_expiration_date rileva una data nel formato corretto.
    
  - Passa il valore di checksum
    
    Nell'esempio seguente, ad esempio attiverà per un criterio di numero di carta di credito DLP:
    
  - Visa: 4485 3647 3952 7352 
    
  - Scadenza: 2/2009
    
Per ulteriori informazioni sul funzionamento di un **Numero di carta di credito** devono essere rilevate per il contenuto, vedere la sezione seguente in questo articolo: [Che cosa the riservati tipi di informazioni cercare carta di credito #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)
  
Utilizzo di un tipo di informazioni riservate predefinite diverse, vedere l'articolo seguente per informazioni su cosa è necessario per altri tipi: [cercare cosa the riservati tipi di informazioni](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

