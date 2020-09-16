---
title: Problemi nell’utilizzo della console di amministrazione di Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 10b37b2ffda50dc77396039a9e0e443ad81aef72
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728291"
---
# <a name="problems-using-the-intune-admin-console"></a><span data-ttu-id="bd005-102">Problemi nell’utilizzo della console di amministrazione di Intune</span><span class="sxs-lookup"><span data-stu-id="bd005-102">Problems using the Intune admin console</span></span>

<span data-ttu-id="bd005-103">**"Accesso negato" durante la navigazione nel portale di amministrazione di Intune.**</span><span class="sxs-lookup"><span data-stu-id="bd005-103">**"Access denied" when navigating the Intune admin portal.**</span></span>

- <span data-ttu-id="bd005-104">Se si è membri di un ruolo personalizzato di Intune, assicurarsi che all'account sia assegnata una licenza di Intune o Enterprise Mobility Suite (EMS).</span><span class="sxs-lookup"><span data-stu-id="bd005-104">If you are a member of an Intune custom role, ensure that an Intune or Enterprise Mobility Suite (EMS) license is assigned to your account.</span></span>
- <span data-ttu-id="bd005-105">Se si usa Configuration Manager per gestire i dispositivi, verificare di non far parte della raccolta di utenti di Intune per Configuration Manager MDM.</span><span class="sxs-lookup"><span data-stu-id="bd005-105">If you are using Configuration Manager to manage devices, verify you are not part of the Intune user collection for Configuration Manager MDM.</span></span>
- <span data-ttu-id="bd005-106">Verificare che siano state assegnate le appropriate autorizzazioni di controllo di amministrazione in base al ruolo nel pannello dei ruoli di Intune.</span><span class="sxs-lookup"><span data-stu-id="bd005-106">Verify that you have been assigned the appropriate role-based administration control (RBAC) permissions in the Intune roles blade.</span></span>
- <span data-ttu-id="bd005-107">Verificare che il gruppo usato non sia una lista di distribuzione.</span><span class="sxs-lookup"><span data-stu-id="bd005-107">Verify the group used is not a distribution list.</span></span> <span data-ttu-id="bd005-108">Intune nel portale di Azure supporta solo gli account utente che appartengono a gruppi di sicurezza di Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="bd005-108">Intune in the Azure portal only supports user accounts that belong to Azure Active Directory security groups.</span></span> <span data-ttu-id="bd005-109">Controllare i gruppi nel portale di Azure > **Intune** > **Gruppi** o nel portale di Azure > **Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="bd005-109">Review your groups in the Azure portal > **Intune** > **Groups**, or in Azure portal > **Azure Active Directory**.</span></span>

<span data-ttu-id="bd005-110">**L’utente ha troppe autorizzazioni per il ruolo di Intune assegnato**</span><span class="sxs-lookup"><span data-stu-id="bd005-110">**User has too many permissions for assigned Intune role**</span></span>

<span data-ttu-id="bd005-111">Consigliare all'utente di passare a **Intune** > **Ruoli di Intune** > **Autorizzazioni personali** > **Esportare** per rivedere le autorizzazioni concesse.</span><span class="sxs-lookup"><span data-stu-id="bd005-111">Advise the user to go to **Intune** > **Intune roles** > **My permissions** > **Export** to review granted permissions.</span></span>

<span data-ttu-id="bd005-112">**È stato aggiunto un gruppo di ambito circoscritto a un ruolo, ma gli utenti in questo ruolo vedono ancora altri utenti o dispositivi.**</span><span class="sxs-lookup"><span data-stu-id="bd005-112">**I added a scope group to a role, but users in that role still see other users or devices.**</span></span>

<span data-ttu-id="bd005-113">I gruppi di ambito circoscritto non filtrano utenti o dispositivi.</span><span class="sxs-lookup"><span data-stu-id="bd005-113">Scope groups do not filter out users or devices.</span></span> <span data-ttu-id="bd005-114">Gruppi di ambito circoscritto:</span><span class="sxs-lookup"><span data-stu-id="bd005-114">Scope groups:</span></span>

- <span data-ttu-id="bd005-115">Limitano le persone alle quali gli utenti possono assegnare criteri o applicazioni.</span><span class="sxs-lookup"><span data-stu-id="bd005-115">Limit who users can assign policies or applications to.</span></span>
- <span data-ttu-id="bd005-116">Consentono solo a specifici utenti di eseguire attività remote sui dispositivi.</span><span class="sxs-lookup"><span data-stu-id="bd005-116">Allow only specific users to run remote tasks on devices.</span></span>

<span data-ttu-id="bd005-117">Per altre informazioni sui gruppi di ambito circoscritto, vedere [Controllo degli accessi in base al ruolo (RBAC) con Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="bd005-117">For more information about scope groups, see  [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="bd005-118">**È stato aggiunto un utente a un ruolo di Intune, ma è comunque possibile l’accesso completo alla console di amministrazione di Intune.**</span><span class="sxs-lookup"><span data-stu-id="bd005-118">**I added a user to an Intune role but they still have full access to the Intune admin console.**</span></span>

<span data-ttu-id="bd005-119">Passare a Intune > **Utenti** nel portale di Azure e verificare che l'utente non sia assegnato ad alcuno dei ruoli seguenti nel portale di Azure:</span><span class="sxs-lookup"><span data-stu-id="bd005-119">Navigate to Intune > **Users** in the Azure portal and verify that the user is not assigned to any of the following roles in the Azure portal:</span></span>

- <span data-ttu-id="bd005-120">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="bd005-120">Global administrator</span></span>
- <span data-ttu-id="bd005-121">Amministratore del servizio Intune</span><span class="sxs-lookup"><span data-stu-id="bd005-121">Intune service administrator</span></span>
- <span data-ttu-id="bd005-122">Amministratore di SharePoint</span><span class="sxs-lookup"><span data-stu-id="bd005-122">SharePoint administrator</span></span>

<span data-ttu-id="bd005-123">Per altre informazioni, vedere [Controllo degli accessi in base al ruolo con Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="bd005-123">For more info, see [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="bd005-124">**Problemi di accesso**</span><span class="sxs-lookup"><span data-stu-id="bd005-124">**Access Issues**</span></span>

<span data-ttu-id="bd005-125">Per altre informazioni, vedere [Non è possibile accedere a Office 365, Azure o Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span><span class="sxs-lookup"><span data-stu-id="bd005-125">For more info, see [You can't sign in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span></span>