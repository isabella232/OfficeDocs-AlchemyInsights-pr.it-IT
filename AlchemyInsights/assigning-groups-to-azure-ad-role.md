---
title: Assegnare gruppi a un ruolo Azure AD
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
- "7898"
- "9003230"
ms.openlocfilehash: feca81fe785bc45e47f6faa876230b5c7701713d
ms.sourcegitcommit: 6dc6f999e840c90694a246b90062950205679420
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 01/15/2021
ms.locfileid: "49875405"
---
# <a name="assigning-groups-to-azure-ad-role"></a><span data-ttu-id="23860-102">Assegnare gruppi a un ruolo Azure AD</span><span class="sxs-lookup"><span data-stu-id="23860-102">Assigning groups to Azure AD role</span></span>

<span data-ttu-id="23860-103">Per assegnare a un gruppo Azure AD un'origine dell'autorità in Azure AD a un ruolo Azure AD, seguire i seguenti passaggi:</span><span class="sxs-lookup"><span data-stu-id="23860-103">To assign an Azure AD group with source of authority in Azure AD to an Azure AD role, perform the following steps:</span></span>

1. <span data-ttu-id="23860-104">Creare un nuovo gruppo - Per creare un nuovo gruppo:</span><span class="sxs-lookup"><span data-stu-id="23860-104">Create a new group - To create a new group:</span></span>

    <span data-ttu-id="23860-105">a.</span><span class="sxs-lookup"><span data-stu-id="23860-105">a.</span></span> <span data-ttu-id="23860-106">Accedere all'interfaccia di amministrazione di Azure AD con un **ruolo di amministratore con privilegi** o con autorizzazioni di **amministratore globale**.</span><span class="sxs-lookup"><span data-stu-id="23860-106">Sign in to the Azure AD admin center with **privileged role administrator** or **global administrator** permissions.</span></span>
    <span data-ttu-id="23860-107">b.</span><span class="sxs-lookup"><span data-stu-id="23860-107">b.</span></span> <span data-ttu-id="23860-108">Selezionare **Azure Active Directory > Groups > Tutti i gruppi > Nuovo gruppo**.</span><span class="sxs-lookup"><span data-stu-id="23860-108">Select **Azure Active Directory > Groups > All groups > New group**.</span></span>
    <span data-ttu-id="23860-109">c.</span><span class="sxs-lookup"><span data-stu-id="23860-109">c.</span></span> <span data-ttu-id="23860-110">Creare il gruppo.</span><span class="sxs-lookup"><span data-stu-id="23860-110">Create the group.</span></span>

2. <span data-ttu-id="23860-111">Assegnare il ruolo al gruppo durante la creazione del gruppo o in seguito alla sua creazione.</span><span class="sxs-lookup"><span data-stu-id="23860-111">Assign the role to the group either during group creation or after the group is created.</span></span>

    <span data-ttu-id="23860-112">a.</span><span class="sxs-lookup"><span data-stu-id="23860-112">a.</span></span> <span data-ttu-id="23860-113">Per assegnare un ruolo al gruppo al momento della creazione del gruppo, passare ad attivare/disattivare **I ruoli Azure AD possono essere assegnati al gruppo** e creare il gruppo.</span><span class="sxs-lookup"><span data-stu-id="23860-113">To assign a role to the group at the time of group creation, switch on the toggle **Azure AD roles can be assigned to the group** and create the group.</span></span>
    <span data-ttu-id="23860-114">b.</span><span class="sxs-lookup"><span data-stu-id="23860-114">b.</span></span> <span data-ttu-id="23860-115">Per assegnare un ruolo al gruppo in seguito alla sua creazione, passare alla scheda **Ruoli assegnati** per il gruppo appena creato e assegnare il ruolo al gruppo.</span><span class="sxs-lookup"><span data-stu-id="23860-115">To assign a role to the group after it has been created, navigate to the **Assigned roles** tab for the newly created group, and assign the role to the group.</span></span>  

<span data-ttu-id="23860-116">**Gestire l'appartenenza di un gruppo a cui è stato assegnato un ruolo Azure AD**</span><span class="sxs-lookup"><span data-stu-id="23860-116">**Manage membership of a group that is assigned to Azure AD role**</span></span>

<span data-ttu-id="23860-117">Per impostazione predefinita, per evitare l'elevazione dei privilegi, solo gli amministratori con ruoli con privilegi e gli amministratori globali possono modificare l'appartenenza di un gruppo a cui sia stato assegnato un ruolo.</span><span class="sxs-lookup"><span data-stu-id="23860-117">To prevent elevation of privileges, by default, only privileged role administrators and global administrators can modify the membership of a group that is assigned to a role.</span></span> <span data-ttu-id="23860-118">Tuttavia, possono scegliere di assegnare un proprietario per tale gruppo e delegare questa attività.</span><span class="sxs-lookup"><span data-stu-id="23860-118">They can, however, choose to assign an owner for such a group and delegate this task.</span></span>

<span data-ttu-id="23860-119">Per ulteriori informazioni sull'assegnazione dei gruppi cloud ai ruoli Azure AD, vedere [Assegnare ruoli AD a un gruppo cloud](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span><span class="sxs-lookup"><span data-stu-id="23860-119">For more details on assigning cloud groups to Azure AD roles, see [Assign a AD roles to Cloud Group](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span></span> <span data-ttu-id="23860-120">Per ulteriori informazioni sulla risoluzione dei problemi dei ruoli assegnati a gruppi cloud, vedere [Risoluzione dei problemi relativi ai ruoli assegnati a gruppi cloud](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span><span class="sxs-lookup"><span data-stu-id="23860-120">For more details on troubleshooting roles assigned to cloud groups, see [Troubleshoot roles assigned to cloud groups](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span></span>





