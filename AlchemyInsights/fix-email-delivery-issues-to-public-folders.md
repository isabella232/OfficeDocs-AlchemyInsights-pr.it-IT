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
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="3d74c-102">Risolvere i problemi di recapito della posta elettronica per le cartelle pubbliche abilitate</span><span class="sxs-lookup"><span data-stu-id="3d74c-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="3d74c-103">Se i mittenti esterni non possono inviare messaggi alle cartelle pubbliche abilitate alla posta elettronica e i mittenti ricevono l'errore: **Impossibile trovare (550 5.4.1)**, verificare che il dominio di posta elettronica per la cartella pubblica sia configurato come dominio di inoltro interno anziché come dominio autorevole:</span><span class="sxs-lookup"><span data-stu-id="3d74c-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="3d74c-104">Aprire l'interfaccia di [amministrazione di Exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="3d74c-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="3d74c-105">Passare a **Mail flow** \> **domini accettati**per il flusso di posta, selezionare il dominio accettato e quindi fare clic su **modifica**.</span><span class="sxs-lookup"><span data-stu-id="3d74c-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="3d74c-106">Nella pagina proprietà che si apre, se il tipo di dominio è impostato su **autorevole**, cambiare il valore in **Relay interno** e quindi fare clic su **Salva**.</span><span class="sxs-lookup"><span data-stu-id="3d74c-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="3d74c-107">Se i mittenti esterni ricevono l'errore **che non si dispone delle autorizzazioni (550 5.7.13)**, eseguire il comando seguente in [PowerShell di Exchange Online](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) per visualizzare le autorizzazioni per gli utenti anonimi nella cartella pubblica:</span><span class="sxs-lookup"><span data-stu-id="3d74c-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="3d74c-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Ad esempio, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span><span class="sxs-lookup"><span data-stu-id="3d74c-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="3d74c-109">Per consentire agli utenti esterni di inviare messaggi di posta elettronica a questa cartella pubblica, aggiungere il diritto di accesso CreateItems all'utente anonimo.</span><span class="sxs-lookup"><span data-stu-id="3d74c-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="3d74c-110">Ad esempio, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span><span class="sxs-lookup"><span data-stu-id="3d74c-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
