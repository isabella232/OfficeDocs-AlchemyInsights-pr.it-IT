---
title: DLP non funziona come previsto
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
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: e1049f160a9b92040095b6725fa5771218a0956d17f99ea8a6e9cc279e7c73f6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54079706"
---
# <a name="dlp-not-working-as-expected"></a>DLP non funziona come previsto

**Importante**: durante questi periodi senza precedenti, stiamo adottando misure per garantire che i servizi SharePoint Online e OneDrive rimangano disponibili. Per altre informazioni, vedere [Modifiche temporanee delle funzionalità di SharePoint Online](https://aka.ms/ODSPAdjustments).

 **Configurazione della prevenzione della perdita dei dati**

Si verificano problemi con la prevenzione della perdita dei dati **(DLP)** Office 365 non funziona come previsto? In tal caso, assicurarsi che il criterio **DLP** sia configurato correttamente e che i dati contengano ciò che il criterio **DLP** sta cercando quando viene valutato.
  
I criteri DLP consentono di identificare e proteggere le informazioni riservate nell'organizzazione. Per configurare i criteri DLP, utilizzare le informazioni [qui](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template).
  
 **Ricerca dei criteri DLP**
  
Quando si utilizzano **i tipi** di informazioni riservate incorporati nei Centri sicurezza e conformità, i criteri DLP ricercano modelli ed elementi specifici durante il rilevamento di questi tipi sensibili.
  
- **Tipi di informazioni riservate incorporati**

    Per informazioni sui tipi sensibili incorporati e sugli elementi cercati da un criterio DLP durante il rilevamento del tipo di dati sensibili, vedere: Ricerca dei tipi di [informazioni riservate](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).

- **Tipi di informazioni riservate personalizzati**

    Se si sta tentando di creare tipi di informazioni riservate personalizzati, utilizzare l'articolo seguente per informazioni su come creare un tipo di informazioni riservate [personalizzato: Creare un tipo di informazioni riservate personalizzato.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)

**Testare un criterio DLP**

Per testare i dati con un tipo di informazioni riservate predefinito o personalizzato, usa l'opzione Tipo di **test** in **Classificazioni**  >  **Tipi di informazioni sensibili.** Per ulteriori informazioni, vedere [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).

 **Report**
  
- Ottenere informazioni dettagliate sui dati sensibili con [i report DLP.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- Visualizzare dettagli specifici dell'evento con un [rapporto operazioni non consentite.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)
