---
title: Regola DLP per SSN non funzionante
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 3f30998fb3bc4c5442e4e1541b87d88ecd7df6eef3a50e719fa5014eb86af39c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004986"
---
# <a name="dlp-issues-with-social-security-numbers"></a>Problemi dlp con i numeri di previdenza sociale

**Importante**: durante questi periodi senza precedenti, stiamo adottando misure per garantire che i servizi SharePoint Online e OneDrive rimangano disponibili. Per altre informazioni, vedere [Modifiche temporanee delle funzionalità di SharePoint Online](https://aka.ms/ODSPAdjustments).

**Problemi dlp con SSN**

Si verificano problemi con la prevenzione della perdita dei dati **(DLP)** che non funziona per il contenuto contenente un numero di previdenza sociale **(SSN)** quando si utilizza un tipo di informazioni riservate in Microsoft 365? In tal caso, verificare che il contenuto contenga le informazioni necessarie per l'aspetto del criterio DLP. 
  
Ad esempio, per un criterio SSN configurato con un livello di probabilità dell'85%, vengono valutati gli elementi seguenti e devono essere rilevati per l'attivazione della regola:
  
- **[Formato:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 cifre, che possono essere formattate o non formattate

- **[Modello:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Quattro funzioni ricercano i nomi SSN in quattro modelli diversi:

  - Func_ssn trova SSN con formattazione forte precedente alla 2011 formattata con trattini o spazi (ddd-dd-dddd OR ddd ddddd)

  - Func_unformatted_ssn trova SSN con formattazione forte precedente alla versione 2011 non formattata come nove cifre consecutive (ddddddddd)

  - Func_randomized_formatted_ssn trova sSN post-2011 formattati con trattini o spazi (ddd-dd-dddd OR ddd ddddd)

  - Func_randomized_unformatted_ssn trova SSN post-2011 non formattati come nove cifre consecutive (ddddddddd)

- **[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** No, non esiste alcun checksum

- **[Definizione:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** Un criterio DLP è sicuro all'85% che sia stato rilevato questo tipo di informazioni riservate se, entro una prossimità di 300 caratteri:

  - La [funzione Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) trova contenuto che corrisponde al modello.

  - Viene trovata una parola chiave da [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn). Esempi di parole chiave includono:  *Social Security, Social Security#, Soc Sec,SSN*  . Ad esempio, l'esempio seguente si attiva per il criterio SSN DLP: **SSN: 489-36-8350**
  
Per ulteriori informazioni su ciò che è necessario per il fatto che i SSN siano rilevati per il contenuto, vedere la sezione seguente in questo articolo: Informazioni sui tipi di informazioni riservate per i [SSN](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
Utilizzando un diverso tipo di informazioni riservate predefinito, vedere l'articolo seguente per informazioni su ciò che è necessario per altri tipi: cosa ricercano i tipi di [informazioni riservate](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  