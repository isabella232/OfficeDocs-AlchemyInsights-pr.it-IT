---
title: Impostazioni dei criteri riunione
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 39151d3a56cc09a8ae2dd77fb7bf1e99066cc77a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825447"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Gestire i criteri riunione in Microsoft Teams

**Nota: l'applicazione delle modifiche ai criteri per gli utenti può richiedere fino a 24 ore.** Potrebbe non essere possibile apportare immediatamente modifiche ai criteri appena creati. attendere 4 ore e tentare di modificare di nuovo un criterio appena creato.

I criteri riunione vengono utilizzati per controllare le funzionalità disponibili per i partecipanti alle riunioni pianificate dagli utenti dell'organizzazione. Alcune funzionalità dei criteri riunione potrebbero non essere ancora implementate nell'interfaccia di amministrazione di Teams (queste sono etichettate come "presto disponibili" nella documentazione). In questo caso, o se viene visualizzato un errore come "Non è possibile aggiornare il criterio in questo momento, ma riprovare in un secondo momento" nell'interfaccia di amministrazione di Microsoft Teams, è consigliabile utilizzare PowerShell per creare o modificare i criteri di riunione di Teams. 

Per ulteriori informazioni sui criteri riunione, vedere le risorse seguenti:

- Per informazioni sulla creazione di criteri, sull'applicazione di modifiche e sull'assegnazione di utenti al criterio, vedere [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).

- Per apportare modifiche ai criteri utilizzando i cmdlet di PowerShell, vedere [Panoramica di PowerShell di Teams.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) 
    - È necessario usare il modulo [PowerShell di Skype for Business per](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) i criteri di riunione di Teams. 
    - Per ulteriori informazioni, vedere la documentazione relativa ai [cmdlet *-CsTeamsMeetingPolicy.](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps)

