---
title: OneDrive errore di accesso AADSTS50011
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003820"
- "6840"
ms.openlocfilehash: 80aafa2aee7213e1b77d274509a7eb9741c20b525ed97f473093ac8c6514f3c7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54112916"
---
# <a name="onedrive-login-error-aadsts50011"></a>OneDrive errore di accesso AADSTS50011

Se viene visualizzato un errore "AADSTS50011: L'URL di risposta specificato nella richiesta non corrisponde alla risposta" quando si accede all'app OneDrive, verificare quanto segue:

La OneDrive deve essere uguale o maggiore della versione 20.052.XXXX.XXXX. Per verificare la versione, fare clic sull'icona OneDrive blu nell'area di notifica, **selezionare Guida & Impostazioni > Impostazioni > Informazioni** su .

La rete potrebbe bloccare il traffico verso **g.live.com** e **oneclient.sfx.ms**. Se il traffico è bloccato, OneDrive non può aggiornarsi. Contattare l'amministratore di rete per assicurarsi di avere accesso a tali URL. [Questi endpoint devono](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) essere raggiungibili per i clienti che usano Microsoft 365 piani.

Se è necessario ottenere manualmente una versione corrente di OneDrive, visitare [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .
