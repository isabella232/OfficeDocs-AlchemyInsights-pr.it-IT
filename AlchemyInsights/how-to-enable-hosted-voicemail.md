---
title: Come abilitare la segreteria telefonica ospitata
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7563"
ms.openlocfilehash: 26eb22054d246a6ca5a2491c68a5d9e4ed90d45b
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/09/2020
ms.locfileid: "49608848"
---
# <a name="how-to-enable-hosted-voicemail"></a>Come abilitare la segreteria telefonica ospitata

Per abilitare la segreteria telefonica, è necessario impostare **HostedVoicemail** su $true.

La proprietà **HostedVoicemail** dell'utente che utilizza Remote PowerShell (RPS).

Per ulteriori informazioni sulla connessione a RPS, vedere [Microsoft teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) per ulteriori informazioni sulla connessione a RPS.

1. È necessario che l'amministratore dei team sia connesso a Remote PowerShell per i team.
1. Dal prompt di PowerShell l'amministratore dei team può eseguire **set-csuser user@contoso.com-HostedVoiceMail $true** in cui l'URI SIP è dell'utente in questione.

> [!NOTE]
> Le modifiche apportate ai criteri possono richiedere fino a 24 ore per la replica.