---
title: Problemi di connessione di SharePoint Designer
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: a4aeaeaea5743c276b907c78317ff30f5610be81
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36508427"
---
# <a name="sharepoint-designer-connection-issues"></a>Problemi di connessione di SharePoint Designer 

Se in SharePoint Designer si verificano problemi di connessione per i siti di SharePoint, provare a eseguire le soluzioni comuni seguenti.

Passaggio 1: verificare che SharePoint Designer 2013 sia stato aggiornato con [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) e l' [aggiornamento del 2 agosto 2016 per SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Passaggio 2: cancellare i file della cache locale:

1. Chiudere SharePoint Designer 2013.

2. Nel computer locale, rimuovere tutti i file trovati in ognuna delle cartelle seguenti.

    - Extensions\Cache del server%APPDATA%\Microsoft\Web
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Aprire SharePoint Designer 2013 e immettere di nuovo l'account per verificare se funziona.

Passaggio 3: [abilitare l'autenticazione moderna per Office 2013 nei dispositivi Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).

Passaggio 4: gli amministratori dovranno **consentire lo script personalizzato** nelle impostazioni dell'interfaccia di amministrazione di SharePoint per consentire la connessione a SharePoint Designer. Per ulteriori informazioni, vedere [Consenti o Impedisci lo script personalizzato](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) .


