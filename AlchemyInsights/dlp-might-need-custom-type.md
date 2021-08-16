---
title: DLP potrebbe richiedere un tipo personalizzato
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 1b0beb89eaf8a4105659a1faa7cc723174a73940ef46bd2355bdddfee7b94adb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030798"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP potrebbe richiedere un tipo personalizzato

**Importante**: durante questi periodi senza precedenti, stiamo adottando misure per garantire che i servizi SharePoint Online e OneDrive rimangano disponibili. Per altre informazioni, vedere [Modifiche temporanee delle funzionalità di SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP potrebbe richiedere un tipo di informazioni personalizzato**

Con un criterio di prevenzione della perdita dei dati (DLP), è possibile identificare e proteggere i dati sensibili nell'organizzazione. In alcuni scenari potrebbe essere necessario creare un **tipo** di informazioni riservate personalizzato per proteggere i dati dell'organizzazione.

Ad esempio, l'organizzazione potrebbe dover identificare e proteggere gli ID dei dipendenti o altri dati in un formato specifico dell'organizzazione. In tal caso, vedere gli articoli seguenti per ulteriori informazioni.
  
 **Personalizzare un tipo di informazioni sensibili predefinito**
  
Se un tipo di informazioni riservate predefinito soddisfa le proprie esigenze con poche modifiche, è possibile personalizzare un tipo di [informazioni riservate predefinito.](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type) Ad esempio, puoi aggiungere o rimuovere parole chiave oppure aggiungere o rimuovere prove di supporto, ad esempio una data o un indirizzo.
  
 **Creare una tipologia personalizzata di informazioni riservate**
  
Tuttavia, se è necessario identificare e proteggere del tutto [](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) un tipo diverso di informazioni riservate, è possibile creare un tipo di informazioni riservate personalizzato nell'interfaccia utente del Centro sicurezza & conformità.
  
**Creare un tipo di informazioni sensibili personalizzato in PowerShell per Centro sicurezza e conformità**

Infine, se l'interfaccia utente non fornisce tutte le opzioni necessarie, è possibile creare un tipo di informazioni riservate personalizzato [in PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell)per centro sicurezza & conformità . A partire da un file XML, è possibile utilizzare tutte le opzioni disponibili.
