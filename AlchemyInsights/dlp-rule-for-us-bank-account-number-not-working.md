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
ms.openlocfilehash: 0b5c1fb175275028c56e47080708520fe115fb38
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932539"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>Problemi DLP con i numeri di conto corrente bancario statunitense

**Importante**: molti clienti di SharePoint Online e OneDrive eseguono applicazioni aziendali critiche rispetto al servizio in esecuzione in background. Tali applicazioni includono soluzioni per la migrazione del contenuto, di Prevenzione della perdita dei dati e per il backup. In questi tempi straordinari, stiamo adottando misure per garantire che i servizi di SharePoint Online e OneDrive rimangano altamente disponibili e affidabili per gli utenti che dipendono ancor più dal servizio negli scenari di lavoro remoto.

A sostegno di questo obiettivo, abbiamo implementato limitazioni più rigide sulle app in background (migrazione, prevenzione della perdita dei dati e soluzioni di backup) durante il giorni nei giorni feriali. In questo periodo sarà possibile notare una riduzione della velocità effettiva in queste app. Tuttavia, nelle ore serali e durante il fine settimana nell'area il servizio sarà predisposto per elaborare una quantità notevolmente superiore di richieste delle app in background.

**Problemi DLP con i numeri di conto corrente bancario statunitense**

Se si riscontrano problemi con la **prevenzione della perdita di dati (DLP),** non funziona per il contenuto contenente un **numero di conto corrente bancario statunitense** quando si utilizza un tipo di informazioni riservate DLP in O365? In caso affermativo, verificare che il contenuto contenga le informazioni necessarie per la ricerca del criterio DLP quando viene valutato.
  
Ad esempio, per un criterio del **numero di conto corrente bancario statunitense** configurato con un livello di probabilità pari a 85%, vengono valutati e devono essere rilevati i seguenti elementi per attivare la regola:
  
- **[Formato:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 cifre

- **[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 cifre consecutive.

- **[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, non c'è nessun checksum

- **[Definizione:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** Un criterio DLP è 75% fiducioso di aver rilevato questo tipo di informazioni riservate se, entro 300 caratteri:

  - L'espressione regolare Regex_usa_bank_account_number trova contenuto che corrisponde al modello

  - Viene trovata una parola chiave da Keyword_usa_Bank_Account.

    Ad esempio, il seguente esempio verrebbe attivato per i criteri del **numero di conto corrente bancario statunitense** : checking account 78344011

Per ulteriori informazioni su ciò che è necessario per il numero di un **conto corrente bancario statunitense** da rilevare per il contenuto, vedere la sezione seguente di questo articolo: [che cosa i tipi di informazioni riservate cercano il numero di conto corrente bancario statunitense](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)
  
Se si utilizza un tipo di informazioni riservate predefinito diverso, vedere l'articolo seguente per informazioni su ciò che è necessario per gli altri tipi: [che cosa cercano i tipi di informazioni riservate](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  