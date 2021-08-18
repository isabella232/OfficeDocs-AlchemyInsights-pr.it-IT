---
title: Risolvere i problemi di installazione di MDATP in un Mac
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4139f47f40a89069521aaa1a3e4fdab56e9e27a2096ae0ad099be827f60d51fc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54091040"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>Risolvere i problemi di installazione di MDATP in un Mac

Se l'installazione manuale non riesce, nella pagina **Riepilogo** dell'installazione guidata viene visualizzato l'errore seguente:

"Si è verificato un errore durante l'installazione. Il programma di installazione ha rilevato un errore che ha causato l'errore dell'installazione. Contattare il produttore del software per assistenza."

Anche per le distribuzioni MDM, la pagina mostra un errore di installazione generico.

Anche se non vengono visualizzati errori esatti per gli utenti finali, microsoft mantiene un file di registro con lo stato di avanzamento dell'installazione, in **/Library/Logs/Microsoft/mdatp/install.log**. Ogni sessione di installazione viene aggiunta a questo file di registro. Per eseguire solo l'output dell'ultima sessione di installazione, utilizzare `sed` .

Per altre informazioni, vedi [Risolvere i problemi di installazione per Microsoft Defender ATP per Mac.](https://go.microsoft.com/fwlink/?linkid=2144615)
