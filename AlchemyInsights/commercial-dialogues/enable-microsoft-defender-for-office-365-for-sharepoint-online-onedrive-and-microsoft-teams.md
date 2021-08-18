---
title: Abilitare Cassaforte allegati per SharePoint Online, OneDrive e Microsoft Teams
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 61372075ac8ccf04606a8003b4ec29f89fc048e5
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332383"
---
# <a name="enable-safe-attachments-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Abilitare Cassaforte allegati per SharePoint Online, OneDrive e Microsoft Teams

1. Usando le credenziali di amministratore globale o amministratore della sicurezza, aprire il portale di Microsoft 365 Defender all'indirizzo e quindi passare a Criteri & regole Criteri di Cassaforte Allegati nella sezione <https://security.microsoft.com>  \>  \>  Criteri 

   Per passare direttamente alla pagina **Cassaforte allegati,** utilizzare <https://security.microsoft.com/safeattachmentv2> .

2. Nella pagina **Cassaforte allegati** fare clic su **Impostazioni globali.**
3. Nel riquadro a comparsa visualizzato seleziona Attiva **Microsoft Defender per Office 365 per SharePoint, OneDrive** e Microsoft Teams e quindi seleziona **Salva.**

    **Suggerimento:** eseguire la procedura seguente per migliorare la protezione degli Cassaforte allegati per SharePoint, OneDrive e Microsoft Teams:
    - Per impedire agli utenti di scaricare file dannosi, utilizzare il valore del parametro `$true` *DisallowInfectedFileDownload* nel cmdlet **[Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant)** in SharePoint PowerShell online. Per ulteriori informazioni, vedere [Use SharePoint Online PowerShell to prevent users from downloading malicious files](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-2-recommended-use-sharepoint-online-powershell-to-prevent-users-from-downloading-malicious-files).
    - [Creare un criterio di avviso per i file rilevati](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-3-recommended-use-the-microsoft-365-defender-portal-to-create-an-alert-policy-for-detected-files)

Per ulteriori informazioni, vedere [Cassaforte allegati per Office 365 per SharePoint, OneDrive e Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041).
