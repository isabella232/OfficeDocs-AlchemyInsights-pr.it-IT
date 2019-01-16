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
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/15/2019
ms.locfileid: "28297006"
---
Si sono verificati problemi con **Prevenzione della perdita di dati (DLP)** non funziona per il contenuto che include un **Numero di conto bancario US** quando si utilizza un tipo di informazioni riservate DLP in Office 365? In tal caso, verificare che il contenuto contiene le informazioni necessarie per quali il criterio DLP è cercando quando viene valutata. 
  
Ad esempio, per un criterio di **Numero di conto bancario US** configurato con un livello di probabilità di 85%, le operazioni seguenti vengono valutati le proprietà e devono essere rilevati della regola da attivare: 
  
- **[Formato:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 17 8 cifre 
    
- **[Motivo:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 17 8 cifre consecutive. 
    
- **[Checksum:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, non esiste alcun Checksum 
    
- **[Definizione:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)** Un criterio DLP è 75% la certezza che è stato rilevato questo tipo di informazioni riservate se all'interno di prossimità di 300 caratteri: 
    
  - L'espressione regolare Regex_usa_bank_account_number individua contenuto corrispondente al formato
    
  - Viene trovata una parola chiave da Keyword_usa_Bank_Account.
    
    Nell'esempio seguente, ad esempio attiverà per il criterio di **Numero di conto bancario negli Stati Uniti** : 78344011 conto corrente 
    
Per ulteriori informazioni sul funzionamento di un **Numero di conto bancario negli Stati Uniti** e rilevato per il contenuto, vedere la sezione seguente in questo articolo: [Che cosa the riservati tipi di informazioni cercare il numero di conto bancario negli Stati Uniti](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)
  
Utilizzo di un tipo di informazioni riservate predefinite diverse, vedere l'articolo seguente per informazioni su cosa è necessario per altri tipi: [cercare cosa the riservati tipi di informazioni](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

