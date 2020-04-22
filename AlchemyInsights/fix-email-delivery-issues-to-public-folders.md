---
title: Risolvere i problemi di recapito della posta elettronica per le cartelle pubbliche abilitate
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: e261fe60843555fa45927b0a6b36e1ccf79fb028
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716356"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Risolvere i problemi di recapito della posta elettronica per le cartelle pubbliche abilitate

Se i mittenti esterni non possono inviare messaggi alle cartelle pubbliche abilitate alla posta elettronica e i mittenti ricevono l'errore: **Impossibile trovare (550 5.4.1)**, verificare che il dominio di posta elettronica per la cartella pubblica sia configurato come dominio di inoltro interno anziché come dominio autorevole:

1. Aprire l'interfaccia di [amministrazione di Exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Passare a **Mail flow** \> **domini accettati**per il flusso di posta, selezionare il dominio accettato e quindi fare clic su **modifica**.

3. Nella pagina proprietà che si apre, se il tipo di dominio è impostato su **autorevole**, cambiare il valore in **Relay interno** e quindi fare clic su **Salva**.

Se i mittenti esterni ricevono l'errore **che non si dispone delle autorizzazioni (550 5.7.13)**, eseguire il comando seguente in [PowerShell di Exchange Online](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) per visualizzare le autorizzazioni per gli utenti anonimi nella cartella pubblica:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Ad esempio, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.

Per consentire agli utenti esterni di inviare messaggi di posta elettronica a questa cartella pubblica, aggiungere il diritto di accesso CreateItems all'utente anonimo. Ad esempio, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.
