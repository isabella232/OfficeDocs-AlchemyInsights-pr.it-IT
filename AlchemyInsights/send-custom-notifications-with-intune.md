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
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="194eb-102">Come inviare notifiche personalizzate agli utenti dei dispositivi iOS e Android gestiti</span><span class="sxs-lookup"><span data-stu-id="194eb-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="194eb-103">Le notifiche personalizzate per Intune vengono elaborate dall'app portale aziendale nel dispositivo di un utente.</span><span class="sxs-lookup"><span data-stu-id="194eb-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="194eb-104">L'app crea quindi la notifica push su quel dispositivo.</span><span class="sxs-lookup"><span data-stu-id="194eb-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="194eb-105">Di seguito sono riportati i prerequisiti per il supporto dei dispositivi per la ricezione di notifiche personalizzate e per l'app per creare la notifica push:</span><span class="sxs-lookup"><span data-stu-id="194eb-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="194eb-106">Il dispositivo deve disporre dell'app portale aziendale installata.</span><span class="sxs-lookup"><span data-stu-id="194eb-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="194eb-107">Il dispositivo deve consentire all'app portale aziendale di inviare notifiche push.</span><span class="sxs-lookup"><span data-stu-id="194eb-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="194eb-108">Quando l'app viene installata o aggiornata, viene richiesto all'utente di consentire le notifiche.</span><span class="sxs-lookup"><span data-stu-id="194eb-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="194eb-109">I dispositivi Android devono avere installato i servizi di Google Play.</span><span class="sxs-lookup"><span data-stu-id="194eb-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="194eb-110">Il dispositivo deve essere registrato con Intune.</span><span class="sxs-lookup"><span data-stu-id="194eb-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="194eb-111">Per ulteriori informazioni, tra cui l'invio di un messaggio, vedere la [documentazione relativa alla funzionalità](https://docs.microsoft.com/intune/custom-notifications).</span><span class="sxs-lookup"><span data-stu-id="194eb-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
