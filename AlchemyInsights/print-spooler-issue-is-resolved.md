---
title: Problema dello spooler di stampa risolto
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 53b1c9a8efa3cc978af8b602c8ed90430042186a
ms.sourcegitcommit: 4265a9e79db6c2a396aa80ec0ebd467bbaadf366
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 07/08/2020
ms.locfileid: "45083950"
---
# <a name="print-spooler-issue-is-resolved"></a>Problema dello spooler di stampa risolto

Se il dispositivo è stato aggiornato con Windows 10, **build sistema operativo 19041.329**, potrebbe riscontrarsi un problema che non consente la stampa con alcune stampanti. Lo spooler di stampa potrebbe generare un errore o chiudersi in modo imprevisto durante il tentativo di stampa e la stampante interessata non genera output. Il problema è stato risolto con la build del sistema operativo **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).  

**Indagine in corso**

Il file Local Security Authority Subsystem Service (LSASS - **Isass.exe**) potrebbe presentare problemi in alcuni dispositivi e restituire il messaggio di errore "Processo di sistema critico, C:\WINDOWS\system32\Isass.exe, non riuscito con codice di stato c0000008. Riavviare il computer.".  **Microsoft si sta occupando del problema e fornirà un aggiornamento in una delle prossime versioni.**

Per altre informazioni, consultare l'articolo sui [problemi noti di Windows 10 versione 2004](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).