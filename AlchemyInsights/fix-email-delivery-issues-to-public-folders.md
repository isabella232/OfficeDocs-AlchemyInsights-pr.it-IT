---
title: Risolvere i problemi di recapito della posta elettronica per le cartelle pubbliche abilitate
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1956
ms.assetid: ''
ms.openlocfilehash: 900b6cc2765937ee005c7e7dce5d33bbdf582601
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/07/2019
ms.locfileid: "34752673"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Risolvere i problemi di recapito della posta elettronica per le cartelle pubbliche abilitate

Se i mittenti esterni non possono inviare messaggi alle cartelle pubbliche abilitate alla posta elettronica e i mittenti ricevono l'errore: **Impossibile trovare (550 5.4.1)**, verificare che il dominio di posta elettronica per la cartella pubblica sia configurato come dominio di inoltro interno anziché come un dominio autorevole:

1. Aprire l'interfaccia di [amministrazione di Exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Passare a **** \> **domini accettati**per il flusso di posta, selezionare il dominio accettato e quindi fare clic su **modifica**.

3. Nella pagina proprietà che si apre, se il tipo di dominio è impostato **** su autorevole, cambiare il valore in **Relay interno** e quindi fare clic su **Salva**.

Se i mittenti esterni ricevono l'errore **che non si dispone delle autorizzazioni (550 5.7.13)**, eseguire il comando seguente in [PowerShell di Exchange Online](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) per visualizzare le autorizzazioni per gli utenti anonimi nella cartella pubblica:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Ad esempio, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.

Per consentire agli utenti esterni di inviare messaggi di posta elettronica a questa cartella pubblica, aggiungere il diritto di accesso CreateItems all'utente anonimo. Ad esempio, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.
