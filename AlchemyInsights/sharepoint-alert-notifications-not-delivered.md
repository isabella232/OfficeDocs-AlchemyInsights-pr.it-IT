---
title: SharePoint notifiche di avviso non recapitate
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: 05bd913098372a57d3061e8c516a6a6b4f0a9bdafde02acc930062d6281d06dd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957905"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a>SharePoint notifiche di avviso non recapitate

Controlla la cartella POSTA INDESIDERATA nel tuo messaggio di posta elettronica, perché a volte potrebbero esserci avvisi.

Determinare **se tutti gli avvisi non vengono recapitati** **o** se non viene recapitato un singolo avviso da un file o una raccolta specifica.

- **I singoli avvisi non vengono recapitati:** se non viene recapitato un singolo avviso da un file o una raccolta specifica, è possibile tentare di eliminarlo e ricrearlo. Vedere [Gestire, visualizzare o eliminare SharePoint avvisi per](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) ricreare l'avviso.
- Tutti gli avvisi non vengono recapitati: se non vengono recapitati tutti gli avvisi di più file o raccolte, visitare il [dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) integrità dei servizi per verificare la presenza di avvisi/eventi imprevisti che potrebbero verificarsi con SharePoint o Exchange. Il problema potrebbe essere relativo alla funzionalità SharePoint di avviso o ai ritardi nei messaggi di posta elettronica tramite Exchange. Sarà anche importante notare se altri messaggi di posta elettronica vengono recapitati e, in caso contrario, il problema è probabilmente con Exchange ritardi.

Domande frequenti sugli avvisi:

- Non è possibile inviare avvisi al gruppo di distribuzione, sono supportati solo i gruppi Di sicurezza e O365.
- Non è possibile personalizzare i modelli di messaggio di posta elettronica degli avvisi. è necessario utilizzare Microsoft FLOW o il flusso di lavoro SharePoint designer per ottenere tali risultati.

## <a name="related-topics"></a>Argomenti correlati

Vuoi provare a Microsoft Flow in SharePoint Online?

- [Creare Flow](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [SharePoint e Flow](https://flow.microsoft.com//blog/sharepoint-and-flow/)
