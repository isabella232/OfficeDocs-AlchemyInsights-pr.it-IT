---
title: Configurazione virtuale con Azure Active Directory Domain Services
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7927"
- "9004397"
ms.openlocfilehash: 7c56e467679f9b9a48cfd7a6f70f7ee148ded3e8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884582"
---
# <a name="virtual-configuration-with-aad-domain-services"></a><span data-ttu-id="fa0a1-102">Configurazione virtuale con Azure Active Directory Domain Services</span><span class="sxs-lookup"><span data-stu-id="fa0a1-102">Virtual configuration with AAD domain services</span></span>

<span data-ttu-id="fa0a1-103">La configurazione virtuale con Azure Active Directory Domain Services comporta i seguenti passaggi:</span><span class="sxs-lookup"><span data-stu-id="fa0a1-103">Virtual configuration with AAD domain services involves the following steps:</span></span> 

1. <span data-ttu-id="fa0a1-104">Controllo dell'integrità del dominio sul portale di Azure https://aka.ms/aadds-health</span><span class="sxs-lookup"><span data-stu-id="fa0a1-104">Checking your domain’s health on the Azure portal https://aka.ms/aadds-health</span></span>
2. <span data-ttu-id="fa0a1-105">Controllo del gruppo di sicurezza di rete per rilevare la presenza di eventuali regole che bloccano le porte necessarie per la sincronizzazione in Azure Active Directory Domain Services sul portale https://aka.ms/aadds-networking</span><span class="sxs-lookup"><span data-stu-id="fa0a1-105">Checking your NSG for rules that block ports needed to synchronize in Azure AD Domain Services on the portal https://aka.ms/aadds-networking</span></span>
3. <span data-ttu-id="fa0a1-106">Verifica che la rete virtuale sia stata distribuita nella stessa area di Azure come dominio gestito da Azure Active Directory Domain Services.</span><span class="sxs-lookup"><span data-stu-id="fa0a1-106">Ensuring that your virtual network is deployed in the same Azure Region as your Azure AD Domain Services-managed domain.</span></span>
4. <span data-ttu-id="fa0a1-107">Verifica che non siano presenti domini disponibili nella rete con lo stesso nome dominio.</span><span class="sxs-lookup"><span data-stu-id="fa0a1-107">Ensuring you don’t have an existent domain with the same domain name available on the virtual network.</span></span>

<span data-ttu-id="fa0a1-108">Per ulteriori considerazioni sulla progettazione sulla rete virtuale di Azure a supporto di Azure Active Directory Domain Services, vedere [Considerazioni sulla rete virtuale](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).</span><span class="sxs-lookup"><span data-stu-id="fa0a1-108">For more details on design consideration on Azure Virtual Network to support AAD domain services, see [Virtual Network Consideration](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).</span></span>

