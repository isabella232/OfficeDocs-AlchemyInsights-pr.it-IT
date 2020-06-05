---
title: Ritardi nella ricezione di avvisi di SharePoint e OneDrive
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 7f1033cec3abec782d1eee3b32128c4c60778913
ms.sourcegitcommit: 8e093114cd31141664e267a7c7b779398d5fdfa8
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/04/2020
ms.locfileid: "44563514"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a>Ritardi nella ricezione di avvisi di SharePoint e OneDrive

- Verificare innanzitutto la cartella posta indesiderata o posta indesiderata nella posta elettronica.
- Se **tutti gli avvisi provenienti da più file o raccolte sono ritardati**, visitare il [dashboard di integrità dei servizi](https://portal.office.com/adminportal/home?ref=/servicehealth) per verificare eventuali avvisi/incidenti che potrebbero verificarsi con SharePoint o Exchange. Il problema potrebbe essere relativo alla funzionalità di avviso di SharePoint o ai ritardi nei messaggi di posta elettronica tramite Exchange. Si noti inoltre se è in corso la recapito di altri messaggi di posta elettronica, altrimenti è probabile che si verifichino ritardi di Exchange.
- Se **un singolo avviso di un file o di una raccolta specifico non viene recapitato**, tentare di eliminarlo e ricrearlo. Per ricreare l'avviso [, vedere gestire, visualizzare o eliminare gli avvisi di SharePoint](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) .

> [!NOTE]
> - Gli avvisi non possono essere inviati a un gruppo di distribuzione. Sono supportati solo i gruppi di sicurezza e di O365.
> - Non è possibile personalizzare i modelli di posta elettronica di avviso. Per ottenere tali operazioni, è necessario utilizzare il flusso di lavoro Microsoft Flow o SharePoint Designer.
