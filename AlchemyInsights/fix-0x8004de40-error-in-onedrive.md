---
title: Correggere 0x8004de40 errore in OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649752"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Correggere 0x8004de40 errore in OneDrive

Se stai eseguendo Windows 7 e ricevi questo errore, aggiorna per abilitare [TLS 1.1 e TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)come protocolli sicuri predefiniti in WinHTTP in Windows .

Se si esegue Windows 10 e si riceve un 0x8004de40 con OneDrive:

- Riavviare il computer interessato mentre si è connessi al dominio Acitve Directory.
- Se un riavvio non risolve il problema, scollegati e ricongiungerti al dispositivo da Azure AD. 

**Nota:** è consigliabile essere nella rete aziendale durante l'esecuzione di questi passaggi. Non eseguire questi passaggi quando non sei connesso all'infrastruttura aziendale (ad esempio, durante i viaggi). 

1. Aprire un prompt dei comandi con privilegi elevati selezionando **Start**, fare clic con il pulsante destro del mouse su Prompt dei **comandi** e quindi scegliere Esegui **come amministratore**.

1. Digitare *dsregcmd /leave* e premere **INVIO.**

1. Al termine, digitare *dsregcmd /join* e premere **INVIO.**

1. Al termine, chiudere il prompt dei comandi.

1. Riavviare il computer ed eseguire l'accesso a OneDrive.