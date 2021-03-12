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
ms.openlocfilehash: 0f07e64c95675a4f6a0aeb6df110fe4e6a21d72f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707814"
---
# <a name="dlp-not-working-as-expected"></a>DLP non funziona come previsto

**Importante**: durante questi periodi senza precedenti, stiamo adottando misure per garantire che i servizi SharePoint Online e OneDrive rimangano disponibili. Per altre informazioni, vedere [Modifiche temporanee delle funzionalità di SharePoint Online](https://aka.ms/ODSPAdjustments).

 **Configurazione della prevenzione della perdita dei dati**

Si verificano problemi con la prevenzione della perdita dei dati **(DLP)** in Office 365 non funziona come previsto? In tal caso, assicurarsi che il criterio **DLP** sia configurato correttamente e che i dati contengano ciò che il criterio **DLP** sta cercando durante la valutazione.
  
I criteri DLP consentono di identificare e proteggere le informazioni riservate nell'organizzazione. Per configurare i criteri DLP, utilizzare le informazioni [riportate di seguito.](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template)
  
 **Ricerca dei criteri DLP**
  
Quando si utilizzano **i tipi** di informazioni riservate predefiniti nei Centri sicurezza e conformità, i criteri DLP ricercano modelli ed elementi specifici quando rilevano questi tipi di dati sensibili.
  
- **Tipi di informazioni riservate predefiniti**

    Per informazioni sui tipi di informazioni sensibili predefiniti e sugli elementi cercati da un criterio DLP per rilevare il tipo di dati sensibili, vedere: Cosa vengono cercati i [tipi di informazioni riservate.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)

- **Tipi di informazioni sensibili personalizzati**

    Se si sta tentando di creare tipi di informazioni sensibili personalizzati, utilizzare l'articolo seguente per informazioni su come creare un tipo di informazioni sensibili personalizzato: Creare un tipo di [informazioni sensibili personalizzato.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)

**Testare un criterio DLP**

Per testare i dati con un tipo di informazioni sensibili predefinito o personalizzato, usare l'opzione Tipo di **test** in **Classificazioni**  >  **Tipi di informazioni sensibili.** Per ulteriori informazioni, vedere [Testare i tipi di informazioni sensibili personalizzati.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center)

 **Report**
  
- Ottenere informazioni dettagliate sui dati sensibili con [i report DLP.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- Visualizzare dettagli specifici dell'evento con un [Rapporto operazioni non consentite.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)
