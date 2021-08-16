---
title: Distribuzione di Teams autonoma o con installazioni di Office nuove o esistenti
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: e8baefafc1c2f9583345779c5ae7a9d3d0e05c4b3b7e1b3a74a9a22f7ceed02a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54102206"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Distribuzione di Teams autonoma o con installazioni di Office nuove o esistenti

Microsoft Teams è ora incluso come parte ***delle*** nuove installazioni di Microsoft 365 Apps for enterprise, Microsoft 365 Apps for business e Office per Mac. Per ulteriori informazioni, vedere [Quando Microsoft Teams essere incluso nelle nuove installazioni di Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Inoltre, a partire dalla versione 1906 nel Canale  corrente, Teams verrà aggiunto alle installazioni esistenti di Microsoft 365 Apps for enterprise (e Microsoft 365 Apps for business) nei dispositivi che eseguono Windows quando si aggiorna l'installazione esistente alla versione più recente. Per ulteriori informazioni, vedere [What about existing installations of Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

> [!NOTE]
> Se non si desidera attendere questa pianificazione dell'implementazione, è possibile distribuire Teams [](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) come autonomo per gli utenti seguendo queste istruzioni oppure è possibile fare in modo che gli utenti installino automaticamente Teams da [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) .

Se l'organizzazione non è pronta per la distribuzione di Teams, sono disponibili i [](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) passaggi [](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) che è possibile eseguire per escludere Teams da installazioni nuove o esistenti di Office.  Se si desidera Teams installazione, ma non si desidera che Teams si avvia automaticamente per l'utente dopo l'installazione, vedere [Prevent Microsoft Teams from starting automatically after installation](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

Per ***disinstallare Teams*** da un dispositivo che esegue Windows, vedere [Uninstall Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Per pulire Microsoft Teams da più computer o utenti di destinazione, vedere Microsoft Teams [pulizia della distribuzione.](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)

Se si usano computer condivisi, Servizi Desktop remoto (RDS) o Virtual Desktop Infrastructure (VDI), vedere Ambienti di computer e [VDI](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams)condivisi con Microsoft Teams .

Se stai usando Office per Mac, vedi Microsoft Teams [installazioni in un Mac.](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)

> [!NOTE]
> Dopo Teams, viene aggiornato automaticamente [](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) ogni due settimane circa con nuove funzionalità e aggiornamenti qualitativi. 