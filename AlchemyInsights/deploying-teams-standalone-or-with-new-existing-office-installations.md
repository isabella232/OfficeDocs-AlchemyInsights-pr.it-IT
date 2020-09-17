---
title: Distribuzione di team come autonomo o con installazioni di Office nuove o esistenti
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
ms.openlocfilehash: c3ca4365abc41509ccf602c5b9046655706840fc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806763"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Distribuzione di team come autonomo o con installazioni di Office nuove o esistenti

Microsoft teams è ora incluso nell'ambito delle ***nuove installazioni*** di Microsoft 365 Apps for Enterprise, Microsoft 365 Apps for business e Office per Mac. Per ulteriori informazioni, vedere [quando Microsoft teams inizierà a essere incluso nelle nuove installazioni di Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Inoltre, a partire dalla versione 1906 nel canale corrente, i team verranno ***aggiunti alle installazioni esistenti*** di Microsoft 365 Apps for Enterprise (e Microsoft 365 Apps for business) su dispositivi che eseguono Windows quando si aggiorna l'installazione esistente alla versione più recente. Per ulteriori informazioni, vedere [What about existing installations of Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

> [!NOTE]
> Se non si desidera attendere questa pianificazione di distribuzione, è possibile distribuire i team come indipendenti per gli utenti [seguendo queste istruzioni](https://docs.microsoft.com/MicrosoftTeams/msi-deployment)   oppure è possibile che gli utenti installino i team da soli  [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) .

Se l'organizzazione non è pronta per la distribuzione di Team, è possibile eseguire la procedura per ***escludere i team*** dalle installazioni di Office [nuove](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) o [esistenti](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) . Se si desidera che i team vengano installati, ma non si desidera che i team vengano avviati automaticamente per l'utente dopo l'installazione, vedere [Impedisci l'avvio automatico di Microsoft teams after installation](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

Per ***disinstallare i team*** da un dispositivo su cui è in esecuzione Windows, vedere [Uninstall Microsoft teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Per pulire Microsoft Teams da più computer o utenti di destinazione, vedere [clean up Deployment di Microsoft teams](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Se si utilizzano computer condivisi, Servizi Desktop remoto (RDS) o Virtual Desktop Infrastructure (VDI), vedere [Shared Computer and VDI Environments with Microsoft teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Se si utilizza Office per Mac, vedere [installazioni di Microsoft teams su un Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> Dopo l'installazione dei team, viene [aggiornata automaticamente](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) ogni due settimane con nuove funzionalità e aggiornamenti di qualità. 