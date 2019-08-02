---
title: Distribuzione di team come autonomo o con installazioni di Office nuove o esistenti
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 08/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 3318e1b17cc99e927e1011f7ca9eca8dec616d59
ms.sourcegitcommit: 4600dd4fb577bf5f5482a24616c2d9a6b81e8052
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/01/2019
ms.locfileid: "36054235"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Distribuzione di team come autonomo o con installazioni di Office nuove o esistenti

Microsoft teams è ora incluso nell'ambito di ***nuove installazioni*** di Office 365 ProPlus, Office 365 business e Office per Mac. Per ulteriori informazioni, vedere [quando Microsoft teams inizierà a essere incluso nelle nuove installazioni di Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-office-365-proplus)

Inoltre, a partire dalla versione 1906 nel canale mensile, i team verranno ***aggiunti alle installazioni esistenti*** di Office 365 ProPlus (e Office 365 business) sui dispositivi che eseguono Windows quando si aggiorna l'installazione esistente alla versione più recente. Per ulteriori informazioni, vedere [What about existing installations of Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-office-365-proplus)

> [!NOTE]
> Se non si desidera attendere questa pianificazione di distribuzione, è possibile distribuire i team come indipendenti per gli utenti [seguendo queste istruzioni](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) oppure è possibile che gli utenti installino i team da [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads)soli.

Se l'organizzazione non è pronta per la distribuzione di Team, è possibile eseguire la procedura per escludere i ***Team*** dalle installazioni di Office [nuove](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus) o [esistenti](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) . Se si desidera che i team vengano installati, ma non si desidera che i team vengano avviati automaticamente per l'utente dopo l'installazione, vedere Impedisci l' [avvio automatico di Microsoft teams after installation](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

Per ***disinstallare i team*** da un dispositivo su cui è in esecuzione Windows, vedere [Uninstall Microsoft teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Per pulire Microsoft Teams da più computer o utenti di destinazione, vedere [clean up Deployment di Microsoft teams](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Se si utilizzano computer condivisi, Servizi Desktop remoto (RDS) o Virtual Desktop Infrastructure (VDI), vedere [Shared Computer and VDI Environments with Microsoft teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Se si utilizza Office per Mac, vedere [installazioni di Microsoft teams su un Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> Dopo l'installazione dei team, viene [aggiornata automaticamente](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) ogni due settimane con nuove funzionalità e aggiornamenti di qualità. 