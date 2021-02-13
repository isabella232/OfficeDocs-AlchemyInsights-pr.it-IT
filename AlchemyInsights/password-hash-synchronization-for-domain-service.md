---
title: Sincronizzazione dell'hash delle password per il servizio di dominio
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 7f138837b720926c5b687285a105eb0417ca5b39
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162943"
---
# <a name="password-hash-synchronization-for-domain-service"></a><span data-ttu-id="2b699-102">Sincronizzazione dell'hash delle password per il servizio di dominio</span><span class="sxs-lookup"><span data-stu-id="2b699-102">Password hash synchronization for domain service</span></span>

<span data-ttu-id="2b699-103">**Se l'istanza di Azure AD DS chiede di abilitare la sincronizzazione hash della password**</span><span class="sxs-lookup"><span data-stu-id="2b699-103">**If your Azure AD DS instance is prompting you to enable password hash synchronization**</span></span>

<span data-ttu-id="2b699-104">Si verifica uno scenario in cui si esegue un ambiente ibrido con gli utenti che si sincronizzano da un ambiente locale di Servizi di dominio Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="2b699-104">You encounter a scenario in which you are running a hybrid environment with users synchronizing from an on-premises Azure Active Directory Domain Services (AD DS) environment.</span></span> <span data-ttu-id="2b699-105">Questo scenario si verifica nonostante la sincronizzazione hash delle password da Active Directory DS locale al tenant di Azure AD.</span><span class="sxs-lookup"><span data-stu-id="2b699-105">This scenario is encountered despite you having password hash synchronization from the on-premises AD DS to your Azure AD tenant.</span></span>

<span data-ttu-id="2b699-106">**Causa**</span><span class="sxs-lookup"><span data-stu-id="2b699-106">**Cause**</span></span>

<span data-ttu-id="2b699-107">Questo problema si verifica perché Azure AD Connect per impostazione predefinita non sincronizza gli hash delle password legacy di New Technology LAN Manager (NTLM) e Kerberos necessari per Azure AD DS.</span><span class="sxs-lookup"><span data-stu-id="2b699-107">This is happening because Azure AD Connect by default does not synchronize legacy New Technology LAN Manager (NTLM) and Kerberos password hashes that are needed for Azure AD DS.</span></span>

<span data-ttu-id="2b699-108">**Soluzione**</span><span class="sxs-lookup"><span data-stu-id="2b699-108">**Workaround**</span></span> 

<span data-ttu-id="2b699-109">È necessario configurare Azure AD Connect per sincronizzare gli hash delle password necessari per l'autenticazione NTLM e Kerberos.</span><span class="sxs-lookup"><span data-stu-id="2b699-109">You would need to configure Azure AD Connect to synchronize those password hashes required for NTLM and Kerberos authentication.</span></span>

<span data-ttu-id="2b699-110">Dopo la configurazione di Azure AD Connect, un evento di creazione di account o di modifica della password locale sincronizza anche gli hash delle password legacy con Azure AD.</span><span class="sxs-lookup"><span data-stu-id="2b699-110">After Azure AD Connect is configured, an on-premises account creation or password change event also then synchronizes the legacy password hashes to Azure AD.</span></span> <span data-ttu-id="2b699-111">Vedere questa [per](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) altre informazioni e per indicazioni su come abilitare la sincronizzazione delle password negli ambienti ibridi di Azure AD DS.</span><span class="sxs-lookup"><span data-stu-id="2b699-111">Please see [here](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) for more information on this and for guidance on how to enable password synchronization in Azure AD DS hybrid environments.</span></span>