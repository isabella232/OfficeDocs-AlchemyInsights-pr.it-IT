---
title: SharePoint Problemi di connessione della finestra di progettazione
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: d55f7c1902bb623900fa74bdae70695b6e04ad84ce7b6ea314db614283ec436d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53942029"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Problemi di connessione della finestra di progettazione 

Se SharePoint Designer riscontra problemi di connessione SharePoint siti, provare le soluzioni comuni seguenti.

Passaggio 1: verificare che SharePoint Designer 2013 sia aggiornato [con SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) e l'aggiornamento del 2 agosto [2016 per SharePoint Designer 2013.](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)



Passaggio 2: cancellare i file della cache locale:

1. Chiudere SharePoint Designer 2013.

2. Nel computer locale, rimuovere tutti i file trovati in ognuna delle cartelle seguenti.

    - %APPDATA%\Microsoft\Web Server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Apri SharePoint Designer 2013 e immetti di nuovo l'account per vedere se funziona.

Passaggio 3: [Abilitare l'autenticazione moderna Office 2013 nei Windows dispositivi](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).

Passaggio 4: gli amministratori dovranno consentire lo **script** personalizzato nelle SharePoint'interfaccia di amministrazione per consentire la connessione SharePoint Designer. Per [ulteriori informazioni, vedere Allow or prevent custom script.](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)


