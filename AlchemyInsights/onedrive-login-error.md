---
title: AADSTS50011 d'Error d'OneDrive login
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003820"
- "6840"
ms.openlocfilehash: 1f906f82e99c322ed953800d54fba5a073eacd10
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/09/2020
ms.locfileid: "48947502"
---
# <a name="onedrive-login-error-aadsts50011"></a><span data-ttu-id="d39d6-102">AADSTS50011 d'Error d'OneDrive login</span><span class="sxs-lookup"><span data-stu-id="d39d6-102">OneDrive login error AADSTS50011</span></span>

<span data-ttu-id="d39d6-103">Se viene visualizzato un messaggio di errore "AADSTS50011: l'URL di risposta specificato nella richiesta non corrisponde alla risposta" quando si accede all'app OneDrive, verificare quanto segue:</span><span class="sxs-lookup"><span data-stu-id="d39d6-103">If you receive an error "AADSTS50011: The reply URL specified in the request does not match the reply" when signing into the OneDrive app, check for the following:</span></span>

<span data-ttu-id="d39d6-104">La versione di OneDrive deve essere uguale o superiore alla versione 20.052. XXXX. XXXX.</span><span class="sxs-lookup"><span data-stu-id="d39d6-104">Your OneDrive version needs to be equal to or greater than version 20.052.XXXX.XXXX.</span></span> <span data-ttu-id="d39d6-105">Per controllare la versione, fare clic sull'icona blu di OneDrive nell'area di notifica, selezionare la **guida & impostazioni > impostazioni >**.</span><span class="sxs-lookup"><span data-stu-id="d39d6-105">To check your version, click on the blue OneDrive icon in the notification area, select **Help & Settings > Settings > About**.</span></span>

<span data-ttu-id="d39d6-106">La rete potrebbe bloccare il traffico a **g.Live.com** e **oneclient.SFX.ms**.</span><span class="sxs-lookup"><span data-stu-id="d39d6-106">Your network might block traffic to **g.live.com** and **oneclient.sfx.ms**.</span></span> <span data-ttu-id="d39d6-107">Se il traffico è bloccato, OneDrive non è in grado di eseguire l'aggiornamento.</span><span class="sxs-lookup"><span data-stu-id="d39d6-107">If that traffic is blocked, OneDrive cannot update itself.</span></span> <span data-ttu-id="d39d6-108">Collaborare con l'amministratore di rete per assicurarsi di avere accesso a tali URL.</span><span class="sxs-lookup"><span data-stu-id="d39d6-108">Work with your network administrator to ensure you have access to those URLs.</span></span> <span data-ttu-id="d39d6-109">[Tali endpoint](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) devono essere raggiungibili per i clienti che utilizzano i piani di Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="d39d6-109">[These endpoints](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) should be reachable for customers using Microsoft 365 plans.</span></span>

<span data-ttu-id="d39d6-110">Se è necessario ottenere manualmente una versione corrente di OneDrive, visitare [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .</span><span class="sxs-lookup"><span data-stu-id="d39d6-110">If you need to manually get a current version of OneDrive, visit [https://aka.ms/getonedrive](https://aka.ms/getonedrive).</span></span>
