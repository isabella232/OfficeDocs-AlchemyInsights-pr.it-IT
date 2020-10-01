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
ms.openlocfilehash: d0363d6bdecdb266a5f4a3a14bd496ede6bb9931
ms.sourcegitcommit: 76b147af688f0dc39878a913a050c0e56af054a8
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/29/2020
ms.locfileid: "48305447"
---
# <a name="configure-endpoint-dlp"></a>Configurare Endpoint DLP

Microsoft Endpoint DLP consente di rafforzare la protezione e il controllo per la prevenzione della perdita dei dati sensibili sui dispositivi Windows 10. Una volta completato l'onboarding dei dispositivi in Gestione dispositivi, è possibile creare criteri di prevenzione della perdita dei dati per applicare azioni di protezione per gli elementi. Esplora attività può essere usato per monitorare le attività per gli elementi sensibili. Per altre informazioni, vedere [Onboarding di dispositivi nella gestione dei dispositivi](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

Per iniziare a usare Endpoint DLP:

- Verificare di avere la licenza per SKU/abbonamenti appropriata. Per altre informazioni, vedere [Licenze per SKU/abbonamenti](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- Verificare le autorizzazioni necessarie per abilitare la gestione dei dispositivi, accedere alla pagina di onboarding, o attivare o disattivare il controllo dei dispositivi. Per altre informazioni, vedere [Autorizzazioni](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- Eseguire l'onboarding dei dispositivi in Gestione dispositivi seguendo la procedura di onboarding dei dispositivi. Se l'opzione Onboarding dispositivi (anteprima) non è presente nelle **Impostazioni** del Centro conformità di M365, verificare di avere la licenza e le autorizzazioni appropriate indicate sopra. Per altre informazioni, vedere [Onboarding di dispositivi](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- Creare i criteri di prevenzione della perdita dei dati per proteggere gli elementi sensibili. Per altre informazioni, vedere [Scenari dei criteri di Endpoint DLP](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).

Per altre informazioni su Microsoft Endpoint DLP, veder [Informazioni sulla prevenzione della perdita di dati degli endpoint di Microsoft 365 (anteprima)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).

**Passaggi importanti per la raccolta dei dati, se serve assistenza:**

1. scaricare MDATP Client Analyzer Preview da [http://aka.ms/betamdatpanalyzer](http://aka.ms/betamdatpanalyzer "http://aka.ms/betamdatpanalyzer")
2. Eseguire lo strumento come amministratore dalla finestra di comando:
3. MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t
4. Quando viene chiesto di immettere il numero di minuti per raccogliere le tracce, immettere il numero di minuti necessari per eseguire lo scenario
5. Eseguire lo scenario

Raccogliere l'output del file ZIP da fornire all'agente di supporto.
