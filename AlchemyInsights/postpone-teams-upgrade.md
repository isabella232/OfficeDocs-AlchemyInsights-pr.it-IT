---
title: Posticipare l'aggiornamento di Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2737"
- "4000006"
ms.openlocfilehash: abbf696b1554743bda188704272bfd85fe6f94e2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51801235"
---
# <a name="how-to-postpone-the-microsoft-driven-teams-upgrade"></a><span data-ttu-id="25b11-102">Come posticipare l'aggiornamento di Teams guidato da Microsoft</span><span class="sxs-lookup"><span data-stu-id="25b11-102">How to postpone the Microsoft-driven Teams upgrade</span></span>

<span data-ttu-id="25b11-103">**Importante:** possiamo risolvere il problema usando una diagnostica di supporto, ma sembra che non si utilizzi la nuova interfaccia di amministrazione.</span><span class="sxs-lookup"><span data-stu-id="25b11-103">**Important**: We can help fix this for you using a support diagnostic, but it looks like you are not using the New Admin Center.</span></span> <span data-ttu-id="25b11-104">Per usare la nuova interfaccia di amministrazione, fai scorrere l'interruttore in alto a destra che indica **la nuova interfaccia di amministrazione** verso destra.</span><span class="sxs-lookup"><span data-stu-id="25b11-104">To use the New Admin Center, slide the toggle in the top right that says **new admin center** to the right.</span></span> <span data-ttu-id="25b11-105">Usando la nuova interfaccia di amministrazione, fare clic sul widget Serve **aiuto?** , digitare "Posticipa l'aggiornamento di Teams", quindi seguire le istruzioni per eseguire la diagnostica.</span><span class="sxs-lookup"><span data-stu-id="25b11-105">Using the New Admin Center, click the **Need Help?** widget, type "Postpone Teams Upgrade", then follow the prompts to run the diagnostic.</span></span>

<span data-ttu-id="25b11-106">Se si riceve una comunicazione su un aggiornamento automatico basato su Microsoft da Skype for Business a Microsoft Teams e si desidera posticipare l'aggiornamento  automatico a una data successiva, l'amministratore globale può accedere al portale di amministrazione di [Teams](https://admin.teams.microsoft.com/dashboard) e, dopo aver selezionato il pulsante Aggiorna stato in Aggiornamento di Microsoft Teams, selezionare il pulsante Posticipa. </span><span class="sxs-lookup"><span data-stu-id="25b11-106">If you received communication about a Microsoft-driven automated upgrade from Skype for Business to Microsoft Teams, and you wish to postpone the automated upgrade to a later date, your Global Admin can log in to the [Teams Admin portal](https://admin.teams.microsoft.com/dashboard) and, after selecting the **Refresh Status** button under Microsoft Teams Upgrade, select the **Postpone** button.</span></span> <span data-ttu-id="25b11-107">Per visualizzare la nuova data per l'aggiornamento automatico del tenant a Microsoft Teams, aggiornare la pagina del portale di amministrazione di Teams.</span><span class="sxs-lookup"><span data-stu-id="25b11-107">To see the new date for your tenant's automated upgrade to Microsoft Teams, refresh the Teams Admin portal page.</span></span>

<span data-ttu-id="25b11-108">**Nota:** Il **pulsante** Posticipa sarà disponibile solo se hai ricevuto la notifica del centro messaggi relativa all'aggiornamento automatico.</span><span class="sxs-lookup"><span data-stu-id="25b11-108">**Note:** The **Postpone** button will only be available if you have received the message center notification regarding the automated upgrade.</span></span> 

<span data-ttu-id="25b11-109">Gli amministratori globali possono anche eseguire [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) per ulteriori informazioni sullo stato corrente dell'aggiornamento.</span><span class="sxs-lookup"><span data-stu-id="25b11-109">Global Admins can also run [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) to learn more about their current upgrade status.</span></span>
