---
title: Impostazioni dei criteri di riunione
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
ms.openlocfilehash: 06395bcc1a631adeaa8abb5ad63b971639f226c19e48203078ba1097d43a50f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53925169"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Gestire i criteri riunione in Microsoft Teams

**Nota: l'applicazione delle modifiche ai criteri per gli utenti può richiedere fino a 24 ore.** Potrebbe non essere possibile apportare immediatamente modifiche ai criteri appena creati. attendere 4 ore e tentare di modificare di nuovo un criterio appena creato.

I criteri per le riunioni vengono usati per controllare le funzionalità disponibili per i partecipanti alle riunioni programmate dagli utenti nell'organizzazione. Alcune funzionalità dei criteri riunione potrebbero non essere ancora implementate nell'interfaccia di amministrazione di Teams (queste sono etichettate come "presto disponibili" nella documentazione). In questo caso, o se viene visualizzato un errore come "Non è possibile aggiornare il criterio in questo momento, ma riprovare più avanti" nell'interfaccia di amministrazione di Microsoft Teams, è consigliabile utilizzare PowerShell per creare o modificare i criteri di riunione di Teams. 

Per ulteriori informazioni sui criteri riunione, vedere le risorse seguenti:

- Per informazioni sulla creazione di criteri, l'applicazione di modifiche e l'assegnazione di utenti al criterio, vedere [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).

- Per apportare modifiche ai criteri utilizzando i cmdlet di PowerShell, [vedere Teams Panoramica di PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) 
    - È necessario utilizzare il modulo [Skype for Business PowerShell per](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) Teams criteri riunione. 
    - Per ulteriori informazioni, vedere la documentazione relativa ai [cmdlet *-CsTeamsMeetingPolicy.](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps)

