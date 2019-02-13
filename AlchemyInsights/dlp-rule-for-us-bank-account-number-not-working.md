---
title: Regole DLP per noi numero di conto bancario non funziona
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 9ebfa6bc09cef9ab7c30bddb4fcb8b6be3ab55a5
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29916420"
---
Si sono verificati problemi con **Prevenzione della perdita di dati (DLP)** non funziona per il contenuto che include un **Numero di conto bancario US** quando si utilizza un tipo di informazioni riservate DLP in Office 365? In tal caso, verificare che il contenuto contiene le informazioni necessarie per quali il criterio DLP è cercando quando viene valutata. 
  
Ad esempio, per un criterio di **Numero di conto bancario US** configurato con un livello di probabilità di 85%, le operazioni seguenti vengono valutati le proprietà e devono essere rilevati della regola da attivare: 
  
- **[Formato:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 17 8 cifre 
    
- **[Motivo:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 17 8 cifre consecutive. 
    
- **[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, non esiste alcun Checksum 
    
- **[Definizione:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** Un criterio DLP è 75% la certezza che è stato rilevato questo tipo di informazioni riservate se all'interno di prossimità di 300 caratteri: 
    
  - L'espressione regolare Regex_usa_bank_account_number individua contenuto corrispondente al formato
    
  - Viene trovata una parola chiave da Keyword_usa_Bank_Account.
    
    Nell'esempio seguente, ad esempio attiverà per il criterio di **Numero di conto bancario negli Stati Uniti** : 78344011 conto corrente 
    
Per ulteriori informazioni sul funzionamento di un **Numero di conto bancario negli Stati Uniti** e rilevato per il contenuto, vedere la sezione seguente in questo articolo: [Che cosa the riservati tipi di informazioni cercare il numero di conto bancario negli Stati Uniti](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)
  
Utilizzo di un tipo di informazioni riservate predefinite diverse, vedere l'articolo seguente per informazioni su cosa è necessario per altri tipi: [cercare cosa the riservati tipi di informazioni](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

