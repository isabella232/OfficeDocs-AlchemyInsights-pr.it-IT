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
ms.openlocfilehash: befb89c28396be3dc60d9d812a0c6aced69bea3c1c48d88a4ab81a34d6c259b0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918995"
---
# <a name="11-call-recording"></a>Registrazione delle chiamate 1:1

Se il **pulsante Avvia** registrazione è disattivato in una chiamata 1:1, è necessario modificare le impostazioni dei criteri per l'utente che ha subito l'impatto. Per controllare l'impostazione del criterio, eseguire la diagnostica per l'utente in impatto digitando **Diag: Teams 1:1 Registrazione chiamata** sopra.     

A partire dal 31 maggio 2021, inizieremo a far rispettare un nuovo Teams criteri di chiamata *AllowCloudRecordingForCalls.* Prima di questa modifica, la registrazione delle chiamate 1:1 è controllata dal criterio *AllowCloudRecording* Teams Riunione. Questa modifica è documentata nel post del Centro messaggi: [(Aggiornato) 1:1 Introduzione ai](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)criteri di registrazione delle chiamate .  

*AllowCloudRecordingForCalls*   l'opzione dei criteri di chiamata è **$False** per impostazione predefinita. Se si preferisce impedire a tutti gli utenti di registrare chiamate 1:1, non è necessario eseguire alcuna azione.  

Per abilitare la registrazione delle chiamate per tutti gli utenti nelle chiamate 1:1, [utilizzare Teams PowerShell](/microsoftteams/teams-powershell-install) per eseguire il cmdlet seguente: 

**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True** 

In alternativa, puoi creare un nuovo criterio e impostare **-AllowCloudRecordingForCalls** su **$true** e assegnare tale criterio agli utenti. 

Per ulteriori informazioni, vedere [1:1 Call Recording Policy Controls Are (Almost!) Qui](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).
