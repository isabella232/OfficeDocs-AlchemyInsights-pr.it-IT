---
title: Criteri di protezione delle applicazioni
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: 929400dcf0ca18ce8f52cb11e5c907064449480e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47716897"
---
# <a name="application-protection-policy"></a>Criteri di protezione delle applicazioni

Se non si ha familiarità con i criteri di protezione delle applicazioni (APP), vedere la [Panoramica dei criteri di protezione delle app](https://docs.microsoft.com/intune/apps/app-protection-policy).

Per iniziare a usare i criteri di protezione delle applicazioni, vedere [Come creare e assegnare criteri di protezione delle app](https://docs.microsoft.com/intune/app-protection-policies).

Requisiti dei criteri di protezione delle applicazioni:

- L'utente ha una licenza di Intune o EMS.
- L'utente appartiene a un gruppo a cui sono assegnati criteri di protezione delle applicazioni.
- Un solo utente aziendale è connesso alle app protette su un dispositivo.
- L'applicazione ha implementato [Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started). Per un elenco delle app che supportano l'SDK, vedere [App protette di Microsoft Intune](https://docs.microsoft.com/intune/apps-supported-intune-apps).

I criteri vengono applicati quando un utente che soddisfa i requisiti precedenti accede a un'app abilitata per Intune SDK. Il modo più semplice per determinare se un criterio viene applicato consiste nel richiedere che l'utente imposti un PIN nel criterio. 

Per altre informazioni, vedere:

[Domande frequenti sulla risoluzione dei problemi relativi a criteri di protezione delle app e MAM](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[Come convalidare la configurazione dei criteri di protezione delle app](https://docs.microsoft.com/intune/app-protection-policies-validate)

[Informazioni sui tempi di recapito dei criteri di protezione delle app](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[Come monitorare i criteri di protezione delle app](https://docs.microsoft.com/intune/app-protection-policies-monitor)