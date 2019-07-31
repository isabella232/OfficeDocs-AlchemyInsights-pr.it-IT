---
title: DLP non funziona come previsto
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 1ea457bd69e7d545cf761a0be849695738b19d8b
ms.sourcegitcommit: d6ea6f4456a582559f27b34c0b9455a86a8e61f1
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/31/2019
ms.locfileid: "35941072"
---
# <a name="dlp-not-working-as-expected"></a>DLP non funziona come previsto

Se si riscontrano problemi con la **prevenzione della perdita di dati (DLP)** in Office 365, non funziona come previsto? In caso affermativo, verificare che i **criteri DLP** siano configurati correttamente e che i dati contengano gli elementi desiderati dal **criterio DLP** quando viene valutato.
  
 **Configurazione di DLP**
  
I criteri DLP consentono di identificare e proteggere le informazioni riservate nell'organizzazione. Per configurare i criteri DLP, utilizzare le informazioni [qui](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).
  
 **Ricerca di criteri DLP**
  
Quando si utilizzano i **tipi di informazioni riservate incorporate** nel centro sicurezza e conformità di Office 365, i criteri DLP cercano modelli ed elementi specifici quando si individuano questi tipi riservati.
  
- **Tipi di informazioni riservate incorporate**

    Per informazioni sui tipi riservati incorporati e sull'aspetto di un criterio DLP per il rilevamento del tipo di dati sensibili, vedere: [cosa cercano i tipi di informazioni riservate](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).

- **Tipi di informazioni riservate personalizzate**

    Se si sta tentando di creare tipi di informazioni riservate personalizzate, utilizzare l'articolo seguente per informazioni su come creare un tipo di riservatezza personalizzato: [creare un tipo di informazioni riservate personalizzato](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).

**Testare un criterio DLP**

Per testare i dati con un tipo di informazioni riservate incorporato o personalizzato, utilizzare l' **opzione tipo di test** in **classificazione** > **tipi di informazioni riservate**. Per ulteriori informazioni, vedere [testare i tipi di informazioni riservate personalizzate](https://docs.microsoft.com/en-us/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).

 **Report**
  
- Ottenere Insight dei dati sensibili con i [report DLP.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)

- Per informazioni dettagliate sull'evento, vedere un [rapporto sulle operazioni](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports)non consentite.
