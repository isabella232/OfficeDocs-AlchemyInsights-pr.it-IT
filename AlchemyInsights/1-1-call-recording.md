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
ms.openlocfilehash: 29383643e6867bca7fd31774a9594b82fdc080bb0e7254141e8c883ad861075e
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/11/2021
ms.locfileid: "57886143"
---
# <a name="11-call-recording"></a>Registrazione delle chiamate 1:1

Se il **pulsante Avvia** registrazione è disattivato in una chiamata 1:1, è necessario modificare le impostazioni dei criteri per l'utente che ha subito l'impatto. Per controllare l'impostazione del criterio, eseguire la diagnostica per l'utente in impatto digitando **Diag: Teams registrazione chiamata 1:1** sopra.     

A partire dal 31 maggio 2021, inizieremo Teams a far rispettare un nuovo criterio di chiamata *AllowCloudRecordingForCalls.* Prima di questa modifica, la registrazione delle chiamate 1:1 è controllata dal criterio *AllowCloudRecording* Teams Meeting Policy. Questa modifica è documentata nel post del Centro messaggi: (Aggiornato) Introduzione ai criteri di registrazione [delle chiamate 1:1](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).  

*AllowCloudRecordingForCalls*   l'opzione dei criteri di chiamata è **impostata $False** per impostazione predefinita. Se si preferisce impedire a tutti gli utenti di registrare chiamate 1:1, non è necessario eseguire alcuna azione.  

Per abilitare la registrazione delle chiamate per tutti gli utenti nelle chiamate 1:1, [utilizzare Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install) per eseguire il cmdlet seguente: 

**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True** 

In alternativa, puoi creare un nuovo criterio e impostare **-AllowCloudRecordingForCalls** su **$true** e assegnare tale criterio agli utenti. 

Per ulteriori informazioni, vedere [1:1 Call Recording Policy Controls Are (Almost!) Qui](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).
