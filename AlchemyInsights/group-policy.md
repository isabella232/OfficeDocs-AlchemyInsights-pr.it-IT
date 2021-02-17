---
title: Criteri di gruppo
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8303"
- "9003234"
ms.openlocfilehash: a829a78bbe947300b6dabb9fdb36088c17809742
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 02/15/2021
ms.locfileid: "50243918"
---
# <a name="group-policy"></a><span data-ttu-id="1477d-102">Criteri di gruppo</span><span class="sxs-lookup"><span data-stu-id="1477d-102">Group policy</span></span>

<span data-ttu-id="1477d-103">Le impostazioni per gli oggetti utente e computer in Azure Active Directory Domain Services (Azure AD DS) sono spesso gestite con oggetti Criteri di gruppo.</span><span class="sxs-lookup"><span data-stu-id="1477d-103">Settings for user and computer objects in Azure Active Directory Domain Services (Azure AD DS) are often managed using Group Policy Objects (GPOs).</span></span> <span data-ttu-id="1477d-104">Azure AD DS include oggetti Criteri di gruppo predefiniti per i contenitori Utenti AAD DC e Computer AAD DC.</span><span class="sxs-lookup"><span data-stu-id="1477d-104">Azure AD DS includes built-in GPOs for the AADDC Users and AADDC Computers containers.</span></span> <span data-ttu-id="1477d-105">È possibile personalizzare questi oggetti Criteri di gruppo predefiniti per configurare criteri di gruppo in base alle esigenze dell'ambiente in uso.</span><span class="sxs-lookup"><span data-stu-id="1477d-105">You can customize these built-in GPOs to configure group policy as needed for your environment.</span></span> <span data-ttu-id="1477d-106">I membri del gruppo di amministratori di Azure AD DC hanno privilegi di amministrazione dei criteri di gruppo nel dominio Azure AD DS e possono anche creare unità organizzative e oggetti Criteri di gruppo personalizzati.</span><span class="sxs-lookup"><span data-stu-id="1477d-106">Members of the Azure AD DC administrators group have group policy administration privileges in the Azure AD DS domain, and can also create custom GPOs and organizational units (OUs).</span></span> <span data-ttu-id="1477d-107">Per altre informazioni sui criteri di gruppo e sul relativo funzionamento, vedere la [panoramica di Criteri di gruppo](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).</span><span class="sxs-lookup"><span data-stu-id="1477d-107">For more information on what group policy is and how it works, see [Group Policy overview](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).</span></span>

<span data-ttu-id="1477d-108">In un ambiente ibrido i criteri di gruppo configurati in un ambiente AD DS locale non vengono sincronizzati con Azure AD DS.</span><span class="sxs-lookup"><span data-stu-id="1477d-108">In a hybrid environment, group policies configured in an on-premises AD DS environment aren't synchronized to Azure AD DS.</span></span> <span data-ttu-id="1477d-109">Per definire le impostazioni di configurazione per utenti o computer in Azure AD DS, modificare uno degli oggetti Criteri di gruppo predefiniti oppure creare un oggetto Criteri di gruppo personalizzato.</span><span class="sxs-lookup"><span data-stu-id="1477d-109">To define configuration settings for users or computers in Azure AD DS, edit one of the default GPOs or create a custom GPO.</span></span>

<span data-ttu-id="1477d-110">L'articolo sulla [gestione di Criteri di gruppo](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) illustra come installare gli strumenti Gestione Criteri di gruppo, come modificare gli oggetti Criteri di gruppo predefiniti e come creare oggetti Criteri di gruppo personalizzati.</span><span class="sxs-lookup"><span data-stu-id="1477d-110">This article [Manage Group Policy](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) shows you how to install the Group Policy Management tools, how ton edit the built-in GPOs, and how to create custom GPOs.</span></span>



