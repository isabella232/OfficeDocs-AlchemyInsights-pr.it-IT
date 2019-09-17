---
title: Inviare notifiche personalizzate con Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.date: 07/31/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000679
ms.openlocfilehash: 1244f07fd56cf603280f1710520a04d579224e44
ms.sourcegitcommit: 16f08d051afca3c6d0de32826324f91cf63ab5ba
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/16/2019
ms.locfileid: "36992317"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Come inviare notifiche personalizzate agli utenti dei dispositivi iOS e Android gestiti

Le notifiche personalizzate per Intune vengono elaborate dall'app portale aziendale nel dispositivo di un utente. L'app crea quindi la notifica push su quel dispositivo.

Di seguito sono riportati i prerequisiti per il supporto dei dispositivi per la ricezione di notifiche personalizzate e per l'app per creare la notifica push:

- Il dispositivo deve disporre dell'app portale aziendale installata.  

- Il dispositivo deve consentire all'app portale aziendale di inviare notifiche push. Quando l'app viene installata o aggiornata, viene richiesto all'utente di consentire le notifiche.

- I dispositivi Android devono avere installato i servizi di Google Play.

- Il dispositivo deve essere registrato con Intune.

Per ulteriori informazioni, tra cui l'invio di un messaggio, vedere la [documentazione relativa alla funzionalità](https://docs.microsoft.com/intune/custom-notifications).
