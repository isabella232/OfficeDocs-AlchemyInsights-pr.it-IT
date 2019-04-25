---
title: Regola DLP per il numero di passaporto US/UK non funzionante
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: bb80ef07364a575f6032bb105cff83cd8f95bd63
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32404385"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problemi relativi ai numeri di passaporto DLP-US/UK

Se si riscontrano problemi con la **prevenzione della perdita di dati (DLP),** non funziona per il contenuto che contiene un **numero di passaporto USA/UK** quando si utilizza un tipo di informazioni riservate DLP in O365? In caso affermativo, verificare che il contenuto contenga le informazioni necessarie per la ricerca del criterio DLP quando viene valutato. 
  
Ad esempio, per un criterio del **numero di passaporto USA/UK** configurato con un livello di confidenza pari al 75%, vengono valutati e devono essere rilevati per la regola da attivare 
  
- **[Formato:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nove cifre 
    
- **[Motivo:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nove cifre consecutive 
    
- **[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, non c'è nessun checksum 
    
- **[Definizione:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** Un criterio DLP è 75% fiducioso di aver rilevato questo tipo di informazioni riservate se, entro 300 caratteri: 
    
  - La funzione Func_usa_uk_passport restituisce contenuti che corrispondono al modello.
    
  - Viene trovata una parola chiave da Keyword_passport.
    
    Ad esempio, il seguente esempio verrebbe attivato per il criterio del **numero di passaporto USA/UK** : US passport Number 123456789 
    
Per ulteriori informazioni su ciò che è necessario per rilevare il numero di passaporto USA/UK per il contenuto, vedere la sezione seguente di questo articolo: [che cosa i tipi di informazioni riservate cercano il numero di passaporto US/UK](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
Se si utilizza un tipo di informazioni riservate predefinito diverso, vedere l'articolo seguente per informazioni su ciò che è necessario per gli altri tipi: [che cosa cercano i tipi di informazioni riservate](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

