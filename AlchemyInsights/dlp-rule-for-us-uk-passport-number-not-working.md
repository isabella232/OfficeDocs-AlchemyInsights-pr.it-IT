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
Si sono verificati problemi con **Prevenzione della perdita di dati (DLP)** non funziona per contenuto contenente un **US / numero di passaporto Regno Unito** quando si utilizza un tipo di informazioni riservate DLP in Office 365? In tal caso, verificare che il contenuto contiene le informazioni necessarie per quali il criterio DLP è cercando quando viene valutata. 
  
Ad esempio, per un **US / numero di passaporto Regno Unito** criterio configurato con un livello di probabilità pari al 75%, i seguenti vengono valutati le proprietà e devono essere rilevati della regola da attivare 
  
- **[Formato:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nove cifre 
    
- **[Motivo:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nove cifre consecutive 
    
- **[Checksum:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, non esiste alcun Checksum 
    
- **[Definizione:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** Un criterio DLP è 75% la certezza che è stato rilevato questo tipo di informazioni riservate se all'interno di prossimità di 300 caratteri: 
    
  - La funzione Func_usa_uk_passport restituisce contenuti che corrispondono al modello.
    
  - Viene trovata una parola chiave da Keyword_passport.
    
    Attiverà, ad esempio, nell'esempio seguente per il **US / numero di passaporto Regno Unito** criteri: numero di passaporto 123456789 
    
Per ulteriori informazioni sul funzionamento di un attributo inglese Americano / numero di passaporto Regno Unito devono essere rilevate per il contenuto, vedere la sezione seguente in questo articolo: [interfaccia cosa the riservati tipi di informazioni per Stati Uniti / numero di passaporto Regno Unito](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
Utilizzo di un tipo di informazioni riservate predefinite diverse, vedere l'articolo seguente per informazioni su cosa è necessario per altri tipi: [cercare cosa the riservati tipi di informazioni](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

