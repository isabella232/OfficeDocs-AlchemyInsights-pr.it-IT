---
title: Correggere le impostazioni dei criteri utente/delle cassette postali
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
ms.openlocfilehash: ca998c453fcb0905b122436f0eea384a9b8a9992
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50737131"
---
# <a name="fix-user-policymailbox-settings"></a>Correggere le impostazioni dei criteri utente/delle cassette postali

Le impostazioni della posta indesiderata nella cassetta postale hanno interessato questo messaggio. Per esaminare le impostazioni, eseguire le operazioni seguenti:

1. Avviare Exchange Management Shell. Per ulteriori informazioni, vedere [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).
2. Eseguire questo comando (utilizzando l'indirizzo di posta elettronica dell'utente):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**
3. Verificare se l'indirizzo di posta elettronica del mittente fa parte di **TrustedSendersAndDomains** **o BlockedSendersAndDomains**. Se l'indirizzo di posta elettronica è in uno degli elenchi, potrebbe essere necessario rimuoverlo. Per ulteriori informazioni, vedere [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).
