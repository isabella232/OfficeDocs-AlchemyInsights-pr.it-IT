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
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="5c969-102">Come inviare notifiche personalizzate agli utenti dei dispositivi iOS e Android gestiti</span><span class="sxs-lookup"><span data-stu-id="5c969-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="5c969-103">Le notifiche personalizzate per Intune vengono elaborate dall'app portale aziendale nel dispositivo di un utente.</span><span class="sxs-lookup"><span data-stu-id="5c969-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="5c969-104">L'app crea quindi la notifica push su quel dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5c969-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="5c969-105">Di seguito sono riportati i prerequisiti per il supporto dei dispositivi per la ricezione di notifiche personalizzate e per l'app per creare la notifica push:</span><span class="sxs-lookup"><span data-stu-id="5c969-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="5c969-106">Il dispositivo deve disporre dell'app portale aziendale installata.</span><span class="sxs-lookup"><span data-stu-id="5c969-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="5c969-107">Il dispositivo deve consentire all'app portale aziendale di inviare notifiche push.</span><span class="sxs-lookup"><span data-stu-id="5c969-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="5c969-108">Quando l'app viene installata o aggiornata, viene richiesto all'utente di consentire le notifiche.</span><span class="sxs-lookup"><span data-stu-id="5c969-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="5c969-109">I dispositivi Android devono avere installato i servizi di Google Play.</span><span class="sxs-lookup"><span data-stu-id="5c969-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="5c969-110">Il dispositivo deve essere registrato con Intune.</span><span class="sxs-lookup"><span data-stu-id="5c969-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="5c969-111">Per ulteriori informazioni, tra cui l'invio di un messaggio, vedere la [documentazione relativa alla funzionalità](https://docs.microsoft.com/intune/custom-notifications).</span><span class="sxs-lookup"><span data-stu-id="5c969-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
