---
title: Registrazione delle chiamate 1:1
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "7648"
ms.openlocfilehash: af09e8805409446a42a62c82aa577ad27f09a17a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50733853"
---
# <a name="11-call-recording"></a>Registrazione delle chiamate 1:1

Gli amministratori devono intervenire ora per continuare a consentire agli utenti di registrare le chiamate 1:1.
 
A partire dal 12 aprile 2021, inizieremo ad applicazione di una nuova opzione dei criteri di chiamata di Teams *AllowCloudRecordingForCalls.* 

Attualmente le funzionalità di registrazione delle chiamate 1:1 sono controllate dall'opzione *AllowCloudRecording* in Criteri riunione di Teams. Se gli utenti sono autorizzati a registrare riunioni di Teams, possono anche registrare chiamate 1:1.

Se si preferisce impedire a tutti gli utenti di registrare chiamate 1:1, non è necessario eseguire alcuna azione. L'opzione del criterio di chiamata *AllowCloudRecordingForCalls* $False per impostazione predefinita.

Questa modifica è documentata nel post del Centro messaggi seguente: (Aggiornato) Introduzione ai criteri di registrazione delle chiamate [1:1](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) Per impostare l'opzione Criteri di chiamata di Teams, è necessario utilizzare [Teams PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-install)

Per abilitare la registrazione delle chiamate nelle chiamate **1:1:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True

**Per disabilitare la registrazione delle chiamate in chiamate 1:1:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False

