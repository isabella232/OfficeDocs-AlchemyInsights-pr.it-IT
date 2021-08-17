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
ms.openlocfilehash: c17408442cec6c0877b7d66bc8a7fd3062eb0e47
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314388"
---
# <a name="11-call-recording"></a>Registrazione delle chiamate 1:1

Se il **pulsante Avvia** registrazione è disattivato in una chiamata 1:1, è necessario modificare le impostazioni dei criteri per l'utente che ha subito l'impatto. Per controllare l'impostazione dei criteri, eseguire la diagnostica per l'utente in impatto digitando **Diag: Teams registrazione chiamata 1:1** sopra.     

A partire dal 31 maggio 2021, inizieremo ad Teams criteri di chiamata *AllowCloudRecordingForCalls.* Prima di questa modifica, la registrazione delle chiamate 1:1 è controllata dal criterio *AllowCloudRecording* Teams Meeting Policy. Questa modifica è documentata nel post del Centro messaggi: (Aggiornato) Introduzione ai criteri di registrazione [delle chiamate 1:1](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).  

*AllowCloudRecordingForCalls*   l'opzione dei criteri di chiamata è **impostata $False** per impostazione predefinita. Se si preferisce impedire a tutti gli utenti di registrare chiamate 1:1, non è necessario eseguire alcuna azione.  

Per abilitare la registrazione delle chiamate per tutti gli utenti nelle chiamate 1:1, [utilizzare Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install) per eseguire il cmdlet seguente: 

**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True** 

In alternativa, puoi creare un nuovo criterio e impostare **-AllowCloudRecordingForCalls** su **$true** e assegnarlo agli utenti. 

Per ulteriori informazioni, vedere [1:1 Call Recording Policy Controls Are (Almost!) Qui](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).
