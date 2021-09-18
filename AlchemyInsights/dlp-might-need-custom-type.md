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
ms.openlocfilehash: c0996e0cc923c13b7de3752ac6534026e8627c51
ms.sourcegitcommit: dcd1c76ced1a0cec27f4cf8d383593760c198424
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/18/2021
ms.locfileid: "59446695"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP potrebbe richiedere un tipo personalizzato

**Importante**: durante questi periodi senza precedenti, stiamo adottando misure per garantire che i servizi SharePoint Online e OneDrive rimangano disponibili. Per altre informazioni, vedere [Modifiche temporanee delle funzionalità di SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP potrebbe richiedere un tipo di informazioni personalizzato**

Con un criterio di prevenzione della perdita dei dati (DLP), è possibile identificare e proteggere i dati sensibili nell'organizzazione. In alcuni scenari potrebbe essere necessario creare un tipo di informazioni riservate personalizzato per proteggere i dati dell'organizzazione. Per ulteriori informazioni, vedere [Informazioni sui tipi di informazioni riservate](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-learn-about) e Sulle definizioni di entità dei tipi di informazioni [riservate.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)

Per ulteriori informazioni su come creare criteri e tipi di informazioni riservate personalizzati, vedere: 

**Personalizzare un tipo di informazioni sensibili predefinito**

Se un tipo di informazioni riservate predefinito soddisfa le proprie esigenze con poche modifiche, vedere Personalizzare un tipo di informazioni [riservate predefinito.](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type) Ad esempio, puoi aggiungere o rimuovere parole chiave oppure aggiungere o rimuovere prove di supporto, ad esempio una data o un indirizzo.

**Creare una tipologia personalizzata di informazioni riservate**

Tuttavia, se è necessario identificare e proteggere completamente un tipo diverso di informazioni riservate, è possibile creare un tipo di informazioni riservate personalizzato nel Centro conformità Microsoft 365. Per ulteriori informazioni, vedere [Introduzione ai tipi di informazioni riservate personalizzati.](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type)

**Creare un tipo di informazioni sensibili personalizzato in PowerShell per Centro sicurezza e conformità**

Infine, se l'interfaccia utente non fornisce tutte le opzioni necessarie, è possibile creare un tipo di informazioni riservate personalizzato in PowerShell del Centro sicurezza & conformità. A partire da un file XML, è possibile utilizzare tutte le opzioni disponibili. Per ulteriori informazioni, vedere [Create a custom sensitive information type using PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).

Per testare prima il criterio in modalità test, vedere [Implementare](https://docs.microsoft.com/microsoft-365/compliance/dlp-learn-about-dlp#implement-policy-in-test-mode) i criteri in modalità test e [Creare, testare e ottimizzare un criterio DLP.](https://docs.microsoft.com/microsoft-365/compliance/create-test-tune-dlp-policy) 