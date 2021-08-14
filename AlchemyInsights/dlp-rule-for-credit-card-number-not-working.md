---
title: Regola DLP per il numero di carta di credito non funzionante
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
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: bd4f200233d5571fc7b01576038e7b3951a07716a7d5948005418d2896291ee5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005094"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>Problemi dlp con i numeri di carta di credito

**Importante**: durante questi periodi senza precedenti, stiamo adottando misure per garantire che i servizi SharePoint Online e OneDrive rimangano disponibili. Per altre informazioni, vedere [Modifiche temporanee delle funzionalità di SharePoint Online](https://aka.ms/ODSPAdjustments).

**Problemi dlp con i numeri di carta di credito**

Si verificano problemi con la prevenzione della perdita  dei dati **(DLP)** che non funziona per il contenuto contenente un numero di carta di credito quando si utilizza un tipo di informazioni riservate DLP in O365? In tal caso, verificare che il contenuto contenga le informazioni necessarie per attivare il criterio DLP quando viene valutato. Ad esempio,  per un criterio della carta di credito configurato con un livello di probabilità dell'85%, vengono valutati gli elementi seguenti e devono essere rilevati per l'attivazione della regola:
  
- **[Formato:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 cifre che possono essere formattate o non formattate (dddddddd) e devono superare il test Luhn.

- **[Modello:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Modello molto complesso e affidabile che rileva le carte di tutte le principali marche in tutto il mondo, tra cui Visa, MasterCard, Discover Card, JCB, American Express, gift card e carte da pranzo.

- **[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Sì, il checksum Luhn

- **[Definizione:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** Un criterio DLP è sicuro all'85% che sia stato rilevato questo tipo di informazioni riservate se, entro una prossimità di 300 caratteri:

  - La funzione Func_credit_card restituisce contenuti che corrispondono al modello.

  - Si verifica una delle situazioni seguenti:

  - Viene trovata una parola chiave da Keyword_cc_verification.

  - Viene trovata una parola chiave Keyword_cc_name ricerca

  - La funzione Func_expiration_date rileva una data nel formato corretto.

  - Il checksum viene superato

    Ad esempio, l'esempio seguente si attiva per un criterio del numero di carta di credito DLP:

  - Visa: 4485 3647 3952 7352
  
  - Scadenza: 2/2009

Per ulteriori informazioni su ciò  che è necessario per il rilevarsi di un numero di carta di credito per il contenuto, vedere la sezione seguente in questo articolo: Che tipo di informazioni riservate cercare Carta [di credito#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
Utilizzando un diverso tipo di informazioni riservate predefinito, vedere l'articolo seguente per informazioni su ciò che è necessario per altri tipi: cosa ricercano i tipi di [informazioni riservate](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  