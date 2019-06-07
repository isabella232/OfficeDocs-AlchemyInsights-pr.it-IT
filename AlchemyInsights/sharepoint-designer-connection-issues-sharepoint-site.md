---
title: Livelli di autorizzazione di SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 356fef8e02f2c1fd9d209c68194685bb0acaa367
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760697"
---
# <a name="sharepoint-designer-connection-issues"></a>Problemi di connessione di SharePoint Designer 

Se in SharePoint Designer si verificano problemi di connessione per i siti di SharePoint, provare a eseguire le soluzioni comuni seguenti.

Passaggio 1: verificare che SharePoint Designer sia stato aggiornato.

- [SharePoint Designer 2013](https://www.microsoft.com/download/details.aspx?id=35491)

- [SharePoint Designer Service Pack 1 (SP1)](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)

- [Aggiornamento per SharePoint Designer 2013 (KB3114721)](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)

Passaggio 2: cancellare i file della cache locale

- Chiudere SharePoint Designer 2013.

- Nel computer locale, passare alla cartella seguente per rimuovere i file memorizzati nella cache.

- Fare clic sul pulsante Start, scegliere Esegui ed eliminare tutti i file trovati in ognuna delle posizioni seguenti.

%APPDATA%\Microsoft\Web server Extensions\Cache%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

Aprire SharePoint Designer 2013 e immettere di nuovo l'account per verificare se funziona.

Passaggio 3: [abilitare l'autenticazione moderna per Office 2013 nei dispositivi Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)

Passaggio 4: è necessario che gli amministratori consentano lo script personalizzato per consentire la connessione di SharePoint Designer.

Per la procedura dettagliata, esempi e considerazioni, vedere [Allow or impedisce script personalizzato](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


