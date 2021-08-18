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
ms.openlocfilehash: 58acaa29f9d0b066cc7be6f6ee57b1806d0e8812b194e20166b133b7715226a8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54086168"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Come inviare notifiche personalizzate agli utenti di dispositivi iOS e Android gestiti

Le notifiche personalizzate per Intune vengono elaborate dall Portale aziendale app sul dispositivo di un utente. L'app crea quindi la notifica push su quel dispositivo.

Di seguito sono riportati i prerequisiti del dispositivo per supportare la ricezione di notifiche personalizzate e per l'app per creare quindi la notifica push:

- Nel dispositivo deve essere installata l Portale aziendale app.  

- Il dispositivo deve consentire all Portale aziendale app di inviare notifiche push. Quando l'app viene installata o aggiornata, richiede all'utente di consentire le notifiche.

- Nei dispositivi Android deve essere installato Google Play Services.

- Il dispositivo deve essere registrato con Intune.

Per ulteriori informazioni su come inviare un messaggio, vedere la documentazione [relativa alle funzionalità](https://docs.microsoft.com/intune/custom-notifications).
