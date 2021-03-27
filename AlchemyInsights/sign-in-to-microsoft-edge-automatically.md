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
- "8333"
- "9004625"
ms.openlocfilehash: 6021991c125f5cb2a33ce8db8fe7717b528bf49b
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398733"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Accedere automaticamente a Microsoft Edge

Microsoft Edge usa l'account predefinito del sistema operativo per accedere automaticamente a un utente in base alla configurazione del dispositivo dell'utente. 

Di seguito sono descritti gli scenari di ogni tipo di configurazione del dispositivo e del relativo processo di accesso utente dipendente:

- **Il dispositivo è ibrido/AAD-J:** questa opzione è disponibile in Windows 10, Windows di livello inferiore e versioni server corrispondenti. Gli utenti hanno eseguito automaticamente l'accesso con i propri account Azure Active Directory (AD).
- **Il dispositivo è aggiunto al** dominio: questa opzione è disponibile in Windows 10, windows di livello inferiore e versioni server corrispondenti. Per impostazione predefinita, gli utenti con account di dominio non vengono connessi automaticamente. per abilitare l'accesso automatico, utilizzare il **criterio ConfigureOnPremisesAccountAutoSignIn.** Per abilitare l'accesso automatico per gli utenti con account Azure AD, prendi in considerazione l'aggiunta ibrida dei dispositivi.
- L'account predefinito del sistema operativo è un **account Microsoft:** questa opzione è disponibile in Windows 10 RS3 (versione 1709, build 10.0.16299) e versioni successive. È improbabile che lo scenario si verifichi nei dispositivi aziendali. Tuttavia, se l'account predefinito del sistema operativo è un account Microsoft, Microsoft Edge accederà automaticamente all'utente con l'account Microsoft.
 
 
