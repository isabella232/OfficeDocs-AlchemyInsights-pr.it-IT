---
title: Accedi automaticamente Microsoft Edge
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
- "8333"
- "9004625"
ms.openlocfilehash: 4e069a1c75caabf3bef7387140edd5650cf966856b888b5c6b5618a603986d6d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050698"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Accedi automaticamente Microsoft Edge

Microsoft Edge l'account predefinito del sistema operativo per accedere automaticamente a un utente in base alla configurazione del dispositivo dell'utente. 

Di seguito sono descritti gli scenari di ogni tipo di configurazione del dispositivo e del relativo processo di accesso utente dipendente:

- **Il dispositivo è ibrido/AAD-J:** questa opzione è disponibile nelle versioni Windows 10, di livello Windows di livello inferiore e nelle versioni server corrispondenti. Gli utenti vengono automaticamente connessi con i Azure Active Directory (AD).
- **Il dispositivo è aggiunto al** dominio: questa opzione è disponibile nelle versioni Windows 10, di livello Windows e delle versioni server corrispondenti. Per impostazione predefinita, gli utenti con account di dominio non vengono connessi automaticamente. per abilitare l'accesso automatico, utilizzare il **criterio ConfigureOnPremisesAccountAutoSignIn.** Per abilitare l'accesso automatico per gli utenti con account Azure AD, prendi in considerazione l'aggiunta ibrida dei dispositivi.
- L'account predefinito del sistema operativo è un **account Microsoft:** questa opzione è disponibile in Windows 10 RS3 (versione 1709, build 10.0.16299) e versioni successive. È improbabile che lo scenario si verifichi nei dispositivi aziendali. Tuttavia, se l'account predefinito del sistema operativo è un account Microsoft, Microsoft Edge accederà automaticamente all'utente con l'account Microsoft.
 
 
