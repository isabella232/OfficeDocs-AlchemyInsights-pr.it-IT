---
title: Correggere le regole di trasporto
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
ms.openlocfilehash: d89283dec427ba3d4f55fc1f180efc13da16ae15c3d5a6c0c06a696faa6df7f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034758"
---
# <a name="fix-transport-rules"></a>Correggere le regole di trasporto

Questo messaggio è stato influenzato da una regola del flusso di posta personalizzata. Per esaminare la regola esatta, eseguire le operazioni seguenti:

1. Nei risultati dell'invio, in **Ulteriori informazioni,** prendere nota del **GUID** o del **nome del criterio.**
2. Avviare Exchange Management Shell. Per ulteriori informazioni, vedere [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).
3. Eseguire questo comando (usando il GUID dall'invio):  **Get-TransportRule -identity "GUID" | fl * Description***
4. Esaminare la descrizione per visualizzare le condizioni configurate che hanno interessato il messaggio.

Per ulteriori informazioni, vedere [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).
