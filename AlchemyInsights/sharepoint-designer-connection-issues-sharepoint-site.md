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
ms.openlocfilehash: 7451cfe957545537298f57feb5b47bd6d43cddbf
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/04/2019
ms.locfileid: "34716896"
---
# <a name="sharepoint-designer-connection-issues"></a>Problemi di connessione di SharePoint Designer 

<p>Se in SharePoint Designer si verificano problemi di connessione per i siti di SharePoint, provare a eseguire le soluzioni comuni seguenti.</p> <p><strong>Passaggio 1:</strong> <strong>Verifica dell'&nbsp; aggiornamento di SharePoint Designer</strong></p> <ul> <li><a href="https://www.microsoft.com/en-us/download/details.aspx?id=35491">SharePoint Designer 2013</a></li> <li><a href="https://support.microsoft.com/en-us/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1">SharePoint Designer Service Pack 1 (SP1)</a></li> <li><a href="https://support.microsoft.com/en-us/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721">Aggiornamento per SharePoint Designer 2013 (KB3114721)</a></li> </ul> <p><strong>Passaggio 2:</strong> <strong>Cancellare i file della cache locale</strong>&nbsp;</p> <ol> <li style="font-weight: 400;">Chiudere SharePoint Designer 2013.&nbsp;</li> <li style="font-weight: 400;">Nel computer locale, passare alla cartella seguente per rimuovere i file memorizzati nella cache.&nbsp;</li> <li style="font-weight: 400;">Fare clic su <strong>Avvia&gt; esecuzione</strong> ed eliminare tutti i file trovati in ognuna delle posizioni seguenti.&nbsp;<br /><br />Extensions\Cache del server%APPDATA%\Microsoft\Web<br />%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache<br />%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</li> <li style="font-weight: 400;">Aprire SharePoint Designer 2013 e immettere di nuovo l'account per verificare se funziona.</li> </ol> <p><strong>Passaggio 3:</strong> <a href="https://docs.microsoft.com/en-us/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=%252fen-us%252farticle%252fEnable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&amp;view=o365-worldwide"> <strong>Abilitare l'autenticazione moderna per Office 2013 nei dispositivi Windows</strong></a>&nbsp;</p> <p><strong>Passaggio 4:</strong> <strong>Gli amministratori dovranno consentire lo script personalizzato per consentire la connessione di SharePoint Designer</strong>.</p> <p>Per la procedura dettagliata, esempi e considerazioni, vedere <a href="https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script">Allow or impedisce script personalizzato</a>.&nbsp;</p>


