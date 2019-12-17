---
title: FIX 0x8004de40 Error in OneDrive
ms.author: pebaum
author: pebaum
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 48b29f57763ca22a71a23b2afddcac0e8e8a95db
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052041"
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