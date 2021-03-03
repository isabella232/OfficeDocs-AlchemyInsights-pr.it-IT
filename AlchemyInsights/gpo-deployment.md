---
title: Distribuzione di oggetti Criteri di gruppo
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "8602"
ms.openlocfilehash: d31f77e70e8456a4076a8146025f1f8ada977a06
ms.sourcegitcommit: 969219d6dff18d86d679d4d8741d1e39e4ce9539
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/03/2021
ms.locfileid: "50417168"
---
# <a name="gpo-deployment"></a><span data-ttu-id="f2181-102">Distribuzione di oggetti Criteri di gruppo</span><span class="sxs-lookup"><span data-stu-id="f2181-102">GPO Deployment</span></span>

<span data-ttu-id="f2181-103">Le impostazioni per gli oggetti utente e computer in Azure Active Directory Domain Services (Azure AD DS) sono spesso gestite con oggetti Criteri di gruppo.</span><span class="sxs-lookup"><span data-stu-id="f2181-103">Settings for user and computer objects in Azure Active Directory Domain Services (Azure AD DS) are often managed using Group Policy Objects (GPOs).</span></span> <span data-ttu-id="f2181-104">Azure AD DS include oggetti Criteri di gruppo predefiniti per i contenitori Utenti AAD DC e Computer AAD DC.</span><span class="sxs-lookup"><span data-stu-id="f2181-104">Azure AD DS includes built-in GPOs for the AADDC Users and AADDC Computers containers.</span></span> <span data-ttu-id="f2181-105">È possibile personalizzare questi oggetti Criteri di gruppo predefiniti per configurare criteri di gruppo in base alle esigenze dell'ambiente in uso.</span><span class="sxs-lookup"><span data-stu-id="f2181-105">You can customize these built-in GPOs to configure group policy as needed for your environment.</span></span> <span data-ttu-id="f2181-106">I membri del gruppo di amministratori di Azure AD DC hanno privilegi di amministrazione dei criteri di gruppo nel dominio Azure AD DS e possono anche creare unità organizzative e oggetti Criteri di gruppo personalizzati.</span><span class="sxs-lookup"><span data-stu-id="f2181-106">Members of the Azure AD DC administrators group have group policy administration privileges in the Azure AD DS domain, and can also create custom GPOs and organizational units (OUs).</span></span> <span data-ttu-id="f2181-107">Per ulteriori informazioni sui Criteri di gruppo e sul suo funzionamento, vedere [Panoramica di Criteri di gruppo.](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))</span><span class="sxs-lookup"><span data-stu-id="f2181-107">For more information on what group policy is and how it works, see [Group Policy Overview](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).</span></span>

<span data-ttu-id="f2181-108">In un ambiente ibrido i criteri di gruppo configurati in un ambiente AD DS locale non vengono sincronizzati con Azure AD DS.</span><span class="sxs-lookup"><span data-stu-id="f2181-108">In a hybrid environment, group policies configured in an on-premises AD DS environment aren't synchronized to Azure AD DS.</span></span> <span data-ttu-id="f2181-109">Per definire le impostazioni di configurazione per utenti o computer in Azure AD DS, modificare uno degli oggetti Criteri di gruppo predefiniti oppure creare un oggetto Criteri di gruppo personalizzato.</span><span class="sxs-lookup"><span data-stu-id="f2181-109">To define configuration settings for users or computers in Azure AD DS, edit one of the default GPOs or create a custom GPO.</span></span>

<span data-ttu-id="f2181-110">L'articolo sulla [gestione di Criteri di gruppo](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) illustra come installare gli strumenti Gestione Criteri di gruppo, come modificare gli oggetti Criteri di gruppo predefiniti e come creare oggetti Criteri di gruppo personalizzati.</span><span class="sxs-lookup"><span data-stu-id="f2181-110">This article [Manage Group Policy](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) shows you how to install the Group Policy Management tools, how ton edit the built-in GPOs, and how to create custom GPOs.</span></span>
