---
title: Regola DLP per il numero di conto corrente bancario statunitense non funzionante
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
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: d19b2dcc29e23fab522159945496165338a117a47bfcfcadf0b93e4e5f14464f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005022"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>Problemi DLP con i numeri di conto corrente bancario statunitense

**Importante**: durante questi periodi senza precedenti, stiamo adottando misure per garantire che i servizi SharePoint Online e OneDrive rimangano disponibili. Per altre informazioni, vedere [Modifiche temporanee delle funzionalità di SharePoint Online](https://aka.ms/ODSPAdjustments).

**Problemi DLP con i numeri di conto corrente bancario statunitense**

Si verificano problemi con la prevenzione della perdita dei dati **(DLP)** che non funziona per il contenuto contenente un **numero** di conto corrente bancario statunitense quando si utilizza un tipo di informazioni riservate DLP in O365? In tal caso, verificare che il contenuto contenga le informazioni necessarie per la ricerca del criterio DLP quando viene valutato.
  
Ad esempio, per un criterio **numero** di conto corrente bancario statunitense configurato con un livello di probabilità dell'85%, vengono valutati gli elementi seguenti e devono essere rilevati per l'attivazione della regola:
  
- **[Formato:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 cifre

- **[Motivo:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 cifre consecutive.

- **[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, non esiste alcun checksum

- **[Definizione:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** Un criterio DLP è sicuro al 75% che sia stato rilevato questo tipo di informazioni riservate se, entro una prossimità di 300 caratteri:

  - L'espressione regolare Regex_usa_bank_account_number trova contenuto che corrisponde al modello

  - Viene trovata una parola chiave da Keyword_usa_Bank_Account.

    Ad esempio, l'esempio seguente viene attivato per il criterio **Numero di conto** corrente bancario statunitense: Controllo dell'account 78344011

Per ulteriori informazioni su ciò  che è necessario per il rilevato numero di conto corrente bancario statunitense per il contenuto, vedere la sezione seguente in questo articolo: Informazioni sui tipi di informazioni riservate per il numero di conto corrente [bancario statunitense](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)
  
Utilizzando un diverso tipo di informazioni riservate predefinito, vedere l'articolo seguente per informazioni su ciò che è necessario per altri tipi: cosa ricercano i tipi di [informazioni riservate](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  