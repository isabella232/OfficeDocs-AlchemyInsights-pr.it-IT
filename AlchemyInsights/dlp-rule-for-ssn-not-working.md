---
title: Regola DLP per il SSN non funzionante
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 0b83a858975ffe1bb70f16a7452a13d57dff5340
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932529"
---
# <a name="dlp-issues-with-social-security-numbers"></a>Problemi DLP con i numeri di previdenza sociale

**Importante**: molti clienti di SharePoint Online e OneDrive eseguono applicazioni aziendali critiche rispetto al servizio in esecuzione in background. Tali applicazioni includono soluzioni per la migrazione del contenuto, di Prevenzione della perdita dei dati e per il backup. In questi tempi straordinari, stiamo adottando misure per garantire che i servizi di SharePoint Online e OneDrive rimangano altamente disponibili e affidabili per gli utenti che dipendono ancor più dal servizio negli scenari di lavoro remoto.

A sostegno di questo obiettivo, abbiamo implementato limitazioni più rigide sulle app in background (migrazione, prevenzione della perdita dei dati e soluzioni di backup) durante il giorni nei giorni feriali. In questo periodo sarà possibile notare una riduzione della velocità effettiva in queste app. Tuttavia, nelle ore serali e durante il fine settimana nell'area il servizio sarà predisposto per elaborare una quantità notevolmente superiore di richieste delle app in background.

**Problemi relativi alla DLP con SNSS**

Se si riscontrano problemi con la **prevenzione della perdita di dati (DLP),** non funziona per i contenuti che contengono un **numero di previdenza sociale (SSN)** quando si utilizza un tipo di informazioni riservate in Office 365? In caso affermativo, verificare che il contenuto contenga le informazioni necessarie per l'aspetto del criterio DLP. 
  
Ad esempio, per i criteri SSN configurati con un livello di confidenza pari al 85%, vengono valutati e devono essere individuati i seguenti per attivare la regola:
  
- **[Formato:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 cifre, che possono essere in un modello formattato o non formattato

- **[Motivo:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Quattro funzioni cercano SNSS in quattro modelli diversi:

  - Func_ssn trova SNSS con una formattazione complessa pre2011 formattata con trattini o spazi (ddd-dd-dddd o ddd dd dddd)

  - Func_unformatted_ssn trova SNSS con una formattazione complessa pre2011 che non è formattata come nove cifre consecutive (ddddddddd)

  - Func_randomized_formatted_ssn trova post-2011 SNSS formattati con trattini o spazi (ddd-dd-dddd o ddd dd dddd)

  - Func_randomized_unformatted_ssn trova post-2011 SNSS che non sono formattati come nove cifre consecutive (ddddddddd)

- **[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, non c'è nessun checksum

- **[Definizione:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** Un criterio DLP è 85% fiducioso di aver rilevato questo tipo di informazioni riservate se, entro 300 caratteri:

  - La [funzione Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) trova contenuto corrispondente al modello.

  - Viene trovata una parola chiave da [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn). Tra gli esempi di parole chiave sono inclusi: *Social Security, Social Security #, SOC sec, SSN* . Ad esempio, il seguente esempio verrebbe attivato per il criterio DLP SSN: **SSN: 489-36-8350**
  
Per ulteriori informazioni su ciò che è necessario per rilevare SNSS per il contenuto, vedere la sezione seguente in questo articolo: [che cosa i tipi di informazioni riservate cercano SNSS](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
Se si utilizza un tipo di informazioni riservate predefinito diverso, vedere l'articolo seguente per informazioni su ciò che è necessario per gli altri tipi: [che cosa cercano i tipi di informazioni riservate](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  