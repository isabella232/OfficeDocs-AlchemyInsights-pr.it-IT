---
title: Regola DLP per il numero di passaporto usa/Regno Unito non funzionante
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
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 85e3ed7fdc221981de13ab6e2ada8adf2a3a80b40ff163981e047cc4a02a1514
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004950"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problemi relativi alla prevenzione della perdita dei dati - Numeri di passaporto usa/Regno Unito

**Importante**: durante questi periodi senza precedenti, stiamo adottando misure per garantire che i servizi SharePoint Online e OneDrive rimangano disponibili. Per altre informazioni, vedere [Modifiche temporanee delle funzionalità di SharePoint Online](https://aka.ms/ODSPAdjustments).

**Problemi DLP con i numeri di passaporto usa/Regno Unito**

Si verificano problemi con la prevenzione della perdita dei dati **(DLP)** che non funziona per il contenuto contenente un numero di passaporto **statunitense/inglese** quando si utilizza un tipo di informazioni riservate DLP in O365? In tal caso, verificare che il contenuto contenga le informazioni necessarie per la ricerca del criterio DLP quando viene valutato.
  
Ad esempio, per un criterio di numero di passaporto **usa/Regno** Unito configurato con un livello di probabilità del 75%, vengono valutati i seguenti elementi e devono essere rilevati perché la regola si attiva
  
- **[Formato:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Nove cifre

- **[Modello:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Nove cifre consecutive

- **[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, non esiste alcun checksum

- **[Definizione:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** Un criterio DLP è sicuro al 75% che sia stato rilevato questo tipo di informazioni riservate se, entro una prossimità di 300 caratteri:

  - La funzione Func_usa_uk_passport restituisce contenuti che corrispondono al modello.

  - Viene trovata una parola chiave da Keyword_passport.

    Ad esempio, l'esempio seguente si attiverebbe per la politica del numero di passaporto **usa/Regno** Unito: numero di passaporto statunitense 123456789

Per ulteriori informazioni su ciò che è necessario per il rilevarsi di un numero di passaporto statunitense/inglese per il contenuto, vedere la sezione seguente in questo articolo: Informazioni sui tipi di informazioni riservate per il numero di passaporto [statunitense/regno unito](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
Utilizzando un diverso tipo di informazioni riservate predefinito, vedere l'articolo seguente per informazioni su ciò che è necessario per altri tipi: cosa ricercano i tipi di [informazioni riservate](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  