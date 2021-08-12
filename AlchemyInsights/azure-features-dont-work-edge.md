---
title: Cosa fare se le funzionalità di Azure non funzionano correttamente in Microsoft Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8315"
- "9004429"
ms.openlocfilehash: aa89cbd58875f418a0a7a9db4b5eb4f0e4c1223a
ms.sourcegitcommit: e9fcd72e64d35f5ba14dfa0fbde39eae20d86cfe
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 07/27/2021
ms.locfileid: "53603296"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>Cosa fare se le funzionalità di Azure non funzionano correttamente in Microsoft Edge

Microsoft Edge presenta problemi noti relativi alle zone di sicurezza che potrebbero influire sul modo in cui gli utenti di Azure accedono all'interfaccia di amministrazione di Windows. Per altre informazioni, vedere [Problemi noti in Edge](https://go.microsoft.com/fwlink/?linkid=2140608). In caso di problemi con l'uso delle funzionalità di Azure con Microsoft Edge, provare a eseguire le operazioni seguenti:

1. Nella **** barra di ricerca del menu Start digitare **opzioni Internet** e quindi selezionare il risultato.
1. In **Proprietà - Internet** selezionare la scheda **Sicurezza**.
1. Selezionare **Siti attendibili** e quindi **Siti**.
1. Aggiungere l'URL del proprio gateway, oltre a <https://login.microsoftonline.com> e <https://login.live.com>, e selezionare **Chiudi**.
1. In **Proprietà - Internet** selezionare la scheda **Privacy**.
1. Nella sezione Blocco popup selezionare **Impostazioni**. Aggiungere l'URL del proprio gateway, nonché <https://login.microsoftonline.com> e <https://login.live.com>, quindi selezionare **Chiudi**.