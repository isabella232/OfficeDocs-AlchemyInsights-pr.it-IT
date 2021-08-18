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
ms.openlocfilehash: 4042e042554f78febff2073fde6f14db72a6d4e0
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58318652"
---
# <a name="how-to-enable-hosted-voicemail"></a>Come abilitare La segreteria telefonica ospitata

Per abilitare La segreteria telefonica, **HostedVoicemail** deve essere impostato su $true.

La **proprietà HostedVoicemail** nell'utente che usa Remote PowerShell (RPS).

Per ulteriori informazioni sulla connessione a RPS, vedere Microsoft Teams Panoramica di [PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) per altre informazioni sulla connessione a RPS.

1. L Teams Admin deve essere connesso a Remote PowerShell per Teams.
1. Dal prompt di PowerShell l'amministratore di Teams può eseguire **set-csuser user@contoso.com -HostedVoiceMail $true** in cui l'URI sip è dell'utente in questione.

**Nota:** la replica delle modifiche ai criteri può richiedere fino a 24 ore.