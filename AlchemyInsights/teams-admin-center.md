---
title: Interfaccia di amministrazione di Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: bb0d757aab05132ff7169ce75009d7012b9a836c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670368"
---
# <a name="teams-admin-center"></a><span data-ttu-id="2d9bc-102">Interfaccia di amministrazione di Teams</span><span class="sxs-lookup"><span data-stu-id="2d9bc-102">Teams Admin Center</span></span>

<span data-ttu-id="2d9bc-103">Informazioni sulla gestione di Teams con l'[interfaccia di amministrazione di Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span><span class="sxs-lookup"><span data-stu-id="2d9bc-103">Learn about managing Teams with the [Teams Admin Center](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span></span>

<span data-ttu-id="2d9bc-104">Se non si riesce ad accedere all'interfaccia di amministrazione di Teams, verificare quanto segue:</span><span class="sxs-lookup"><span data-stu-id="2d9bc-104">If you are unable to access the Teams Admin Center, please check the following items:</span></span>

- <span data-ttu-id="2d9bc-105">Verificare di avere consentito [gli indirizzi IP e gli URL di Office 365](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) appropriati su tutti i dispositivi perimetrali (firewall e così via) o nelle regole firewall nel computer locale.</span><span class="sxs-lookup"><span data-stu-id="2d9bc-105">Verify that you have allowed the appropriate [Office 365 IP addresses and URL's](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) on any perimeter devices (firewall, etc.) or in the firewall rules on your local machine.</span></span>
- <span data-ttu-id="2d9bc-106">Verificare che l'account usato per accedere al portale di amministrazione di Teams corrisponda al nome utente indicato nel [portale di amministrazione di Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span><span class="sxs-lookup"><span data-stu-id="2d9bc-106">Verify that the login you are using to access the Teams Admin Portal matches your username listed in the [Microsoft 365 Admin portal](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>

<span data-ttu-id="2d9bc-107">Se gli utenti non sono visualizzati nell'interfaccia di amministrazione di Teams, verificare quanto segue:</span><span class="sxs-lookup"><span data-stu-id="2d9bc-107">If users are not appearing in the Teams Admin Center, please check the following:</span></span>

- <span data-ttu-id="2d9bc-108">Sono stati creati utenti o sono state assegnate licenze nelle ultime 24 ore?</span><span class="sxs-lookup"><span data-stu-id="2d9bc-108">Have you created users or assigned licenses in the last 24 hours?</span></span> <span data-ttu-id="2d9bc-109">Attendere almeno 24 ore prima di aprire un ticket di supporto.</span><span class="sxs-lookup"><span data-stu-id="2d9bc-109">Please make sure you wait at least 24 hours before opening a support ticket.</span></span>
- <span data-ttu-id="2d9bc-110">Sono state assegnate le licenze appropriate?</span><span class="sxs-lookup"><span data-stu-id="2d9bc-110">Verify you have assigned appropriate licenses?</span></span>
- <span data-ttu-id="2d9bc-111">Se si dispone di una directory di Active Directory locale, verificare che [il valore di msRTCSIP-PrimaryUserAddress o l'indirizzo SIP nel campo ProxyAddresses in Active Directory locale sia univoco e che il formato corrisponda al](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) SIP:**Nome utente** dell'utente dall' [interfaccia di amministrazione di Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span><span class="sxs-lookup"><span data-stu-id="2d9bc-111">If you have an on-premise Active Directory, verify that [the value of msRTCSIP-PrimaryUserAddress or the SIP address in the ProxyAddresses field in your local Active Directory is unique and the format matches](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) sip:**Username** of the user from the [Microsoft 365 admin center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>
- <span data-ttu-id="2d9bc-112">Se si prevede di mantenere una distribuzione di Skype for Business Server e di avere utenti locali e online: seguire le **"Configurazione ibrida con Teams e Skype for Business online"** nel pannello di controllo di Skype for Business Server e spostare gli utenti online.</span><span class="sxs-lookup"><span data-stu-id="2d9bc-112">If you intend to keep a Skype for Business Server deployment and have users homed on-premises and Online: follow the **"Set up hybrid with Teams and Skype for Business Online"** in your Skype for Business Server Control Panel and move users Online.</span></span>
