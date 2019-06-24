---
title: FIX 0x8004de40 Error in OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 2256fb66cb7a4e2adcff9fda16a80c87e2997f0c
ms.sourcegitcommit: 8f6a1be929b275faa295ba8aeeae17898a47c3b0
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/21/2019
ms.locfileid: "35133981"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>FIX 0x8004de40 Error in OneDrive

Se viene visualizzato un errore di 0x8004de40 con OneDrive:

- Riavviare il computer coinvolto quando si è connessi al dominio di directory di Acitve.
- Se un riavvio non risolve il problema, disconnettersi e riaggiungere il dispositivo da Azure AD. 

**Nota**: durante l'esecuzione di questa procedura, è necessario essere presenti nella rete aziendale. Non eseguire questi passaggi se non si è in grado di connettersi all'infrastruttura aziendale, ad esempio durante il viaggio. 

- Aprire un prompt dei comandi con privilegi elevati. 
- Per aprire un prompt dei comandi con privilegi elevati, fare clic su **Start**, fare clic con il pulsante destro del mouse su **prompt dei comandi**e quindi scegliere **Esegui come amministratore**.
- Digitare *dsregcmd/Leave* e premere **invio**.
- Al termine, digitare *dsregcmd/join* e premere **invio**.
- Al termine, chiudere la finestra del prompt dei comandi.
- Riavviare il computer ed eseguire l'accesso a OneDrive.