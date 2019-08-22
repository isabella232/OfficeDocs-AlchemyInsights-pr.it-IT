---
title: Regola DLP per il numero di conto corrente bancario statunitense non funzionante
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 0a32708b5ac8d95ec6777ada2d151a15f90d65bf
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529875"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>Problemi DLP con i numeri di conto corrente bancario statunitense

Se si riscontrano problemi con la **prevenzione della perdita di dati (DLP),** non funziona per il contenuto contenente un **numero di conto corrente bancario statunitense** quando si utilizza un tipo di informazioni riservate DLP in O365? In caso affermativo, verificare che il contenuto contenga le informazioni necessarie per la ricerca del criterio DLP quando viene valutato.
  
Ad esempio, per un criterio del **numero di conto corrente bancario statunitense** configurato con un livello di probabilità pari a 85%, vengono valutati e devono essere rilevati i seguenti elementi per attivare la regola:
  
- **[Formato:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 cifre

- **[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 cifre consecutive.

- **[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, non c'è nessun checksum

- **[Definizione:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** Un criterio DLP è 75% fiducioso di aver rilevato questo tipo di informazioni riservate se, entro 300 caratteri:

  - L'espressione regolare Regex_usa_bank_account_number trova il contenuto che corrisponde al modello

  - Viene trovata una parola chiave da Keyword_usa_Bank_Account.

    Ad esempio, il seguente esempio verrebbe attivato per i criteri del **numero di conto corrente bancario statunitense** : checking account 78344011

Per ulteriori informazioni su ciò che è necessario per il numero di un **conto corrente bancario statunitense** da rilevare per il contenuto, vedere la sezione seguente di questo articolo: [che cosa i tipi di informazioni riservate cercano il numero di conto corrente bancario statunitense](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)
  
Se si utilizza un tipo di informazioni riservate predefinito diverso, vedere l'articolo seguente per informazioni su ciò che è necessario per gli altri tipi: [che cosa cercano i tipi di informazioni riservate](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  