---
title: Risolvere i problemi di recapito della posta elettronica alle cartelle pubbliche abilitate alla posta
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: ff1400f694ae037a8658356af068b4c20b8fa9d9908dafedb90db7bb6859530f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068816"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Risolvere i problemi di recapito della posta elettronica alle cartelle pubbliche abilitate alla posta

Se i mittenti esterni non possono inviare messaggi alle cartelle pubbliche abilitate alla posta e i mittenti ricevono l'errore: impossibile trovare **(550 5.4.1),** verificare che il dominio di posta elettronica per la cartella pubblica sia configurato come dominio di inoltro interno anziché come dominio autorevole:

1. Aprire [l'Exchange di amministrazione (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Vai a **Flusso di posta** Domini \> **accettati,** seleziona il dominio accettato e quindi fai clic su **Modifica.**

3. Nella pagina delle proprietà visualizzata, se il tipo di dominio è impostato su **Autorevole,** modificare il valore in **Inoltro** interno e quindi fare clic su **Salva**.

Se i mittenti esterni ricevono l'errore che non si dispone **dell'autorizzazione (550 5.7.13),** eseguire il comando seguente [in Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) per visualizzare le autorizzazioni per gli utenti anonimi nella cartella pubblica:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Ad esempio, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .

Per consentire agli utenti esterni di inviare messaggi di posta elettronica a questa cartella pubblica, aggiungere il diritto di accesso CreateItems all'utente Anonimo. Ad esempio, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.
