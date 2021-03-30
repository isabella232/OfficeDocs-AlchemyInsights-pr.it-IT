---
title: Risoluzione dei problemi di Aggiunta ad Azure AD ibrido
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/06/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6162"
- "6158"
- "9003244"
- "9003246"
ms.openlocfilehash: 18d0ce6bdf3df96e07cc6607b9ae6142d548dabe
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 03/29/2021
ms.locfileid: "51401911"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a><span data-ttu-id="214d9-102">Risoluzione dei problemi di Aggiunta ad Azure AD ibrido</span><span class="sxs-lookup"><span data-stu-id="214d9-102">Troubleshoot Hybrid Azure AD join</span></span>

<span data-ttu-id="214d9-103">È consigliabile verificare che un dispositivo possa accedere agli endpoint di registrazione dispositivo nell'account di sistema usando lo [script di Test Device Registration Connectivity](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).</span><span class="sxs-lookup"><span data-stu-id="214d9-103">Highly Recommended Ensure that a device can access Device Registration endpoints under the system account by using the [Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).</span></span>

1. <span data-ttu-id="214d9-104">Se si stanno configurando le registrazioni dei dispositivi per la prima volta, è necessario rivedere [Introduzione alla gestione dei dispositivi in Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) per informazioni su come impostare i dispositivi sotto il controllo di Azure AD.</span><span class="sxs-lookup"><span data-stu-id="214d9-104">If you are setting up device registrations for the first time, be sure to review I[ntroduction to device management in Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) to learn how to get devices under the control of Azure AD.</span></span>
1. <span data-ttu-id="214d9-105">Se i dispositivi vengono registrati direttamente in Azure AD e si sta eseguendo l’iscrizione di questi in Intune, assicurarsi, prima di tutto, di aver [configurato Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) e avere le [licenze](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="214d9-105">If you are registering devices into Azure AD directly and enrolling them into Intune, be sure that you've [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
1. <span data-ttu-id="214d9-106">Assicurarsi di essere autorizzati a eseguire operazioni in Azure AD e Active Directory locale.</span><span class="sxs-lookup"><span data-stu-id="214d9-106">Ensure that you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="214d9-107">Solo l’amministratore globale in Azure AD può gestire le impostazioni per la registrazione dei dispositivi.</span><span class="sxs-lookup"><span data-stu-id="214d9-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="214d9-108">Inoltre, è necessario essere un amministratore di Active Directory e AD FS, se applicabile, se si stanno configurando le registrazioni automatiche in Active Directory locale.</span><span class="sxs-lookup"><span data-stu-id="214d9-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="214d9-109">Per altre informazioni sulla risoluzione di potenziali problemi con l’aggiunta ibrida, vedere [Risoluzione dei problemi di aggiunta ibrida](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current). Per la configurazione di dispositivi aggiunti ad Azure AD ibrido e la gestione dei dispositivi tramite il portale di Azure AD, vedere [Configurare dispositivi aggiunti ad Azure AD ibrido (aggiunto a un dominio locale)](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) e [Gestire i dispositivi usando il portale di Azure](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="214d9-109">For more details on resolve potential issues with Hybrid join, see [Troubleshoot Hybrid Join](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) for set up hybrid Azure AD joined and Manage Devices using Azure Ad portal, see [Set up hybrid Azure AD joined (on-premises domain-joined) devices](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) and [Manage devices using the Azure portal](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="214d9-110">Per risolvere i problemi più comuni di Aggiunta ad Azure Active Directory (AD) ibrido, vedere le [domande frequenti su Aggiunta ad Azure AD ibrido](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).</span><span class="sxs-lookup"><span data-stu-id="214d9-110">To resolve common issues with Hybrid Azure Active Directory (AD) join, see [Hybrid Azure AD join FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).</span></span>
