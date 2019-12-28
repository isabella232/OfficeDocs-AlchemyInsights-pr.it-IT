---
title: Inviare notifiche personalizzate con Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 969649084a2ac536ee1b41f225c3be5415a27c4b
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/27/2019
ms.locfileid: "40886861"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Come inviare notifiche personalizzate agli utenti dei dispositivi iOS e Android gestiti

Le notifiche personalizzate per Intune vengono elaborate dall'app portale aziendale nel dispositivo di un utente. L'app crea quindi la notifica push su quel dispositivo.

Di seguito sono riportati i prerequisiti per il supporto dei dispositivi per la ricezione di notifiche personalizzate e per l'app per creare la notifica push:

- Il dispositivo deve disporre dell'app portale aziendale installata.  

- Il dispositivo deve consentire all'app portale aziendale di inviare notifiche push. Quando l'app viene installata o aggiornata, viene richiesto all'utente di consentire le notifiche.

- I dispositivi Android devono avere installato i servizi di Google Play.

- Il dispositivo deve essere registrato con Intune.

Per ulteriori informazioni, tra cui l'invio di un messaggio, vedere la [documentazione relativa alla funzionalità](https://docs.microsoft.com/intune/custom-notifications).
