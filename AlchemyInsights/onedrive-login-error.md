---
title: AADSTS50011 d'Error d'OneDrive login
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
ms.openlocfilehash: 1f906f82e99c322ed953800d54fba5a073eacd10
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/09/2020
ms.locfileid: "48947502"
---
# <a name="onedrive-login-error-aadsts50011"></a>AADSTS50011 d'Error d'OneDrive login

Se viene visualizzato un messaggio di errore "AADSTS50011: l'URL di risposta specificato nella richiesta non corrisponde alla risposta" quando si accede all'app OneDrive, verificare quanto segue:

La versione di OneDrive deve essere uguale o superiore alla versione 20.052. XXXX. XXXX. Per controllare la versione, fare clic sull'icona blu di OneDrive nell'area di notifica, selezionare la **guida & impostazioni > impostazioni >**.

La rete potrebbe bloccare il traffico a **g.Live.com** e **oneclient.SFX.ms**. Se il traffico è bloccato, OneDrive non è in grado di eseguire l'aggiornamento. Collaborare con l'amministratore di rete per assicurarsi di avere accesso a tali URL. [Tali endpoint](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) devono essere raggiungibili per i clienti che utilizzano i piani di Microsoft 365.

Se è necessario ottenere manualmente una versione corrente di OneDrive, visitare [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .
