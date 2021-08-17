---
title: Come abilitare La segreteria telefonica ospitata
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
ms.openlocfilehash: 4d70e92a7c1bf8f3cc62d4a310aa140ee2dfdef4c798ae17faa961736d9db500
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54055558"
---
# <a name="how-to-enable-hosted-voicemail"></a>Come abilitare La segreteria telefonica ospitata

Per abilitare la segreteria telefonica, **HostedVoicemail** deve essere impostato su $true.

La **proprietà HostedVoicemail** nell'utente che usa Remote PowerShell (RPS).

Per ulteriori informazioni sulla connessione a RPS, vedere Microsoft Teams Panoramica di [PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) per altre informazioni sulla connessione a RPS.

1. L Teams Admin deve essere connesso a Remote PowerShell per Teams.
1. Dal prompt di PowerShell l'amministratore Teams può eseguire **set-csuser user@contoso.com -HostedVoiceMail $true** in cui l'URI sip è dell'utente in questione.

> [!NOTE]
> La replica delle modifiche ai criteri può richiedere fino a 24 ore.