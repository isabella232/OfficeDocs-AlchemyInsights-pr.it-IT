---
title: Accedere automaticamente a Microsoft Edge
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
ms.openlocfilehash: 68a1119abd0a3f687b6448bb6e58c6485c239c0f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/08/2020
ms.locfileid: "49599469"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Accedere automaticamente a Microsoft Edge

Microsoft Edge utilizza l'account predefinito del sistema operativo per accedere automaticamente a un utente in base al modo in cui viene configurato il dispositivo dell'utente. 

Di seguito sono descritti gli scenari di ogni tipo di configurazione del dispositivo e del relativo processo di accesso dell'utente dipendente:

1. **Il dispositivo è ibrido/AAD-J**: questa opzione è disponibile in Windows 10, finestre di livello basso e versioni del server corrispondenti. Gli utenti vengono automaticamente firmati con gli account di Azure Active Directory (AD).
2. **Il dispositivo è associato a un dominio**: questa opzione è disponibile in Windows 10, finestre di livello basso e versioni del server corrispondenti. Per impostazione predefinita, gli utenti con account di dominio non sono firmati automaticamente. per abilitare l'accesso automatico per gli stessi, utilizzare il criterio **ConfigureOnPremisesAccountAutoSignIn** . Per abilitare l'accesso automatico per gli utenti con account Azure AD, prendere in considerazione l'aggiunta ibrida dei propri dispositivi.
3. **L'account predefinito del sistema operativo è un account Microsoft**: questa opzione è disponibile in Windows 10 RS3 (versione 1709, Build 10.0.16299) e versioni successive. Lo scenario è improbabile che si verifichi nei dispositivi Enterprise. Tuttavia, se l'account predefinito del sistema operativo è un account Microsoft, Microsoft Edge accederà automaticamente all'utente con l'account Microsoft.
 
 
