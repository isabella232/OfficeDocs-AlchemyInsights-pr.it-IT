---
title: Teams installato con gli aggiornamenti di Office
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
- "2599"
- "9000140"
- "9000660"
- "2509"
ms.openlocfilehash: 36b0b1a7bf37c27304b4124157dba9aba337678c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51832386"
---
# <a name="microsoft-teams-installed-with-office-updates"></a>Microsoft Teams installato con gli aggiornamenti di Office

Microsoft Teams è incluso ***nell'ambito*** delle nuove installazioni di Microsoft 365 Apps for enterprise, Microsoft 365 Apps for business e Office per Mac. Per ulteriori informazioni, vedere Quando Microsoft Teams inizierà a [essere incluso nelle nuove installazioni di Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Inoltre, a partire dalla versione 1906 nel Canale  corrente, Teams verrà gradualmente aggiunto alle installazioni esistenti di Microsoft 365 Apps for enterprise (e Microsoft 365 Apps for business) nei dispositivi che eseguono Windows quando si aggiorna l'installazione esistente alla versione più recente. Per ulteriori informazioni, vedere [Informazioni sulle installazioni esistenti di Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

**Nota:** Se non si desidera attendere questa pianificazione dell'implementazione, è possibile distribuire Teams come autonomo per gli utenti seguendo queste istruzioni [oppure](https://docs.microsoft.com/MicrosoftTeams/msi-deployment)è possibile fare in modo che gli utenti installino Teams autonomamente da https://teams.microsoft.com/downloads .

Se l'organizzazione non è pronta per distribuire Teams, è possibile ***escludere Teams*** dalle [installazioni](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) nuove [o](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) esistenti di Office. Se si desidera che Teams sia installato, ma non si desidera che Teams si avvia automaticamente per l'utente dopo l'installazione, vedere Impedire l'avvio automatico di [Microsoft Teams dopo l'installazione.](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)

Per ***disinstallare Teams*** da un dispositivo che esegue Windows, vedere [Disinstallare Microsoft Teams.](https://support.office.com/article/uninstall-microsoft-teams-3b159754-3c26-4952-abe7-57d27f5f4c81) Per pulire Microsoft Teams da più computer o utenti di destinazione, vedere [Pulizia della distribuzione di Microsoft Teams.](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)

Se si usano computer condivisi, Servizi Desktop remoto (RDS) o Virtual Desktop Infrastructure (VDI), vedere [Shared computer and VDI environments with Microsoft Teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams). Se si usa Office per Mac, vedere [Installazioni di Microsoft Teams in un Mac.](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)

**Nota:** Dopo l'installazione di Teams, viene [aggiornato automaticamente ogni](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) due settimane circa con nuove funzionalità e aggiornamenti qualitativi. 