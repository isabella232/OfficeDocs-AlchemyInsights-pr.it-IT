---
title: Regola DLP per il numero di passaporto US/UK non funzionante
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: bc91af8be58d49204f84cd7d22f481348af3c013
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529923"
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
  