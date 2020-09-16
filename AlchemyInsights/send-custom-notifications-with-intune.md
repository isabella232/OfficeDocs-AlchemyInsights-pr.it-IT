---
title: Inviare notifiche personalizzate con Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 2e5e2e2f24c46d3db4f08862dcc80934937f6f51
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720650"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Come inviare notifiche personalizzate agli utenti dei dispositivi iOS e Android gestiti

Le notifiche personalizzate per Intune vengono elaborate dall'app portale aziendale nel dispositivo di un utente. L'app crea quindi la notifica push su quel dispositivo.

Di seguito sono riportati i prerequisiti per il supporto dei dispositivi per la ricezione di notifiche personalizzate e per l'app per creare la notifica push:

- Il dispositivo deve disporre dell'app portale aziendale installata.  

- Il dispositivo deve consentire all'app portale aziendale di inviare notifiche push. Quando l'app viene installata o aggiornata, viene richiesto all'utente di consentire le notifiche.

- I dispositivi Android devono avere installato i servizi di Google Play.

- Il dispositivo deve essere registrato con Intune.

Per ulteriori informazioni, tra cui l'invio di un messaggio, vedere la [documentazione relativa alla funzionalità](https://docs.microsoft.com/intune/custom-notifications).
