---
title: Regola DLP per il numero di carta di credito non funzionante
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 6b28534d072c024a98a9b05f6cb55bfdc3435db6
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932447"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>Problemi relativi alla DLP con numeri di carta di credito

**Importante**: molti clienti di SharePoint Online e OneDrive eseguono applicazioni aziendali critiche rispetto al servizio in esecuzione in background. Tali applicazioni includono soluzioni per la migrazione del contenuto, di Prevenzione della perdita dei dati e per il backup. In questi tempi straordinari, stiamo adottando misure per garantire che i servizi di SharePoint Online e OneDrive rimangano altamente disponibili e affidabili per gli utenti che dipendono ancor più dal servizio negli scenari di lavoro remoto.

A sostegno di questo obiettivo, abbiamo implementato limitazioni più rigide sulle app in background (migrazione, prevenzione della perdita dei dati e soluzioni di backup) durante il giorni nei giorni feriali. In questo periodo sarà possibile notare una riduzione della velocità effettiva in queste app. Tuttavia, nelle ore serali e durante il fine settimana nell'area il servizio sarà predisposto per elaborare una quantità notevolmente superiore di richieste delle app in background.

**Problemi relativi alla DLP con numeri di carta di credito**

Se si riscontrano problemi con la **prevenzione della perdita di dati (DLP),** non funziona per il contenuto contenente un **numero di carta di credito** quando si utilizza un tipo di informazioni riservate DLP in O365? In caso affermativo, verificare che il contenuto contenga le informazioni necessarie per attivare il criterio DLP quando viene valutato. Ad esempio, per i **criteri delle carte di credito** configurati con un livello di confidenza pari al 85%, vengono valutati e devono essere rilevati i seguenti elementi per attivare la regola:
  
- **[Formato:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 cifre che possono essere formattate o non formattate (dddddddddddddddd) e devono superare il test di Luhn.

- **[Motivo:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Modello molto complesso e robusto che rileva le schede di tutte le principali marche di tutto il mondo, tra cui Visa, MasterCard, Discover Card, JCB, American Express, Gift Cards e Diner Cards.

- **[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Sì, il checksum di Luhn

- **[Definizione:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Un criterio DLP è 85% fiducioso di aver rilevato questo tipo di informazioni riservate se, entro 300 caratteri:

  - La funzione Func_credit_card restituisce contenuti che corrispondono al modello.

  - Si verifica una delle situazioni seguenti:

  - Viene trovata una parola chiave da Keyword_cc_verification.

  - Viene trovata una parola chiave da Keyword_cc_name

  - La funzione Func_expiration_date rileva una data nel formato corretto.

  - Il checksum passa

    Ad esempio, il seguente esempio si innescherà per un criterio di numero di carta di credito DLP:

  - Visa: 4485 3647 3952 7352
  
  - Scade: 2/2009

Per ulteriori informazioni su ciò che è necessario affinché venga rilevato un **numero di carta di credito** per il contenuto, vedere la sezione seguente di questo articolo: informazioni sui [tipi di informazione sensibili ricerca per la carta di credito](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number) .
  
Se si utilizza un tipo di informazioni riservate predefinito diverso, vedere l'articolo seguente per informazioni su ciò che è necessario per gli altri tipi: [che cosa cercano i tipi di informazioni riservate](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  