---
title: Configurare Endpoint DLP
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 97a8d4e7db9aac65e6a505c0bef8b41d2ea23353
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323922"
---
# <a name="configure-endpoint-dlp"></a>Configurare Endpoint DLP

Microsoft Endpoint DLP consente di rafforzare la protezione e il controllo per la prevenzione della perdita dei dati sensibili sui dispositivi Windows 10. Una volta completato l'onboarding dei dispositivi in Gestione dispositivi, è possibile creare criteri di prevenzione della perdita dei dati per applicare azioni di protezione per gli elementi. Esplora attività può essere usato per monitorare le attività per gli elementi sensibili. Per altre informazioni, vedere [Onboarding di dispositivi nella gestione dei dispositivi](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

Per iniziare a usare Endpoint DLP:

- Verificare di avere la licenza per SKU/abbonamenti appropriata. Per altre informazioni, vedere [Licenze per SKU/abbonamenti](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- Verificare le autorizzazioni necessarie per abilitare la gestione dei dispositivi, accedere alla pagina di onboarding, o attivare o disattivare il controllo dei dispositivi. Per altre informazioni, vedere [Autorizzazioni](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- Eseguire l'onboarding dei dispositivi in Gestione dispositivi seguendo la procedura di onboarding dei dispositivi. Per altre informazioni, vedere [Onboarding di dispositivi](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- Creare i criteri di prevenzione della perdita dei dati per proteggere gli elementi sensibili. Per altre informazioni, vedere [Scenari dei criteri di Endpoint DLP](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).

Per altre informazioni su Microsoft Endpoint DLP, veder [Informazioni sulla prevenzione della perdita di dati degli endpoint di Microsoft 365 (anteprima)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).

**Passaggi importanti per la raccolta dei dati, se serve assistenza:**

1. Scaricare [MDATP Client Analyzer Preview](https://aka.ms/betamdatpanalyzer).
1. Eseguire lo strumento come amministratore dalla finestra di comando:

    **MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**

1. Quando viene richiesto, **Immettere il numero di minuti per raccogliere le tracce:**, immettere il numero di minuti necessari per eseguire lo scenario.
1. Eseguire lo scenario.

Raccogliere l'output del file ZIP da fornire all'agente di supporto.
