---
title: Ruolo di gestione delle identità con privilegi
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
- "9003230"
- "6825"
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086380"
---
# <a name="privileged-identity-managementpim-role"></a><span data-ttu-id="03b7c-102">Ruolo di gestione delle identità privilegiate (PIM)</span><span class="sxs-lookup"><span data-stu-id="03b7c-102">Privileged Identity Management(PIM) role</span></span>

<span data-ttu-id="03b7c-103">**Le autorizzazioni non vengono concesse dopo l'attivazione di un ruolo**</span><span class="sxs-lookup"><span data-stu-id="03b7c-103">**Permissions are not granted after activating a role**</span></span>

<span data-ttu-id="03b7c-104">Quando si attiva un ruolo in Azure AD Privileged Identity Management (PIM), l'attivazione potrebbe non essere immediatamente propagata a tutti i portali che richiedono il ruolo privilegiato.</span><span class="sxs-lookup"><span data-stu-id="03b7c-104">When you activate a role in Azure AD Privileged Identity Management (PIM), the activation may not instantly propagate to all portals that require the privileged role.</span></span> <span data-ttu-id="03b7c-105">A volte, anche se la modifica viene propagata, la memorizzazione nella cache Web in un portale può comportare la modifica che non avrà effetto immediato.</span><span class="sxs-lookup"><span data-stu-id="03b7c-105">Sometimes, even if the change is propagated, web caching in a portal may result in the change not taking effect immediately.</span></span>

<span data-ttu-id="03b7c-106">Se l'attivazione è ritardata, eseguire la procedura seguente:</span><span class="sxs-lookup"><span data-stu-id="03b7c-106">If your activation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="03b7c-107">Disconnettersi dal portale di Azure e quindi eseguire di nuovo l'accesso.</span><span class="sxs-lookup"><span data-stu-id="03b7c-107">Sign out of the Azure portal and then sign back in.</span></span> <span data-ttu-id="03b7c-108">Quando si attiva un ruolo di Azure AD o un ruolo risorsa di Azure, vengono visualizzate le fasi dell'attivazione.</span><span class="sxs-lookup"><span data-stu-id="03b7c-108">When you activate an Azure AD role or an Azure resource role, you will see the stages of your activation.</span></span> <span data-ttu-id="03b7c-109">Una volta completate tutte le fasi, verrà visualizzato il collegamento "Esci".</span><span class="sxs-lookup"><span data-stu-id="03b7c-109">Once all the stages are complete, you will see a 'Sign out' link.</span></span> <span data-ttu-id="03b7c-110">È possibile utilizzare questo collegamento per disconnettersi. Questo risolverà la maggior parte dei casi per il ritardo di attivazione.</span><span class="sxs-lookup"><span data-stu-id="03b7c-110">You can use this link to sign out. This will solve most cases for activation delay.</span></span>
2. <span data-ttu-id="03b7c-111">In PIM, verificare che sia elencato come membro del ruolo.</span><span class="sxs-lookup"><span data-stu-id="03b7c-111">In PIM, verify that you are listed as the member of the role.</span></span>
3. <span data-ttu-id="03b7c-112">Se si sta attivando il ruolo di amministratore di Exchange, assicurarsi di disconnettersi e di accedere nuovamente.</span><span class="sxs-lookup"><span data-stu-id="03b7c-112">If you are activating the Exchange Administrator role, make sure you sign out and sign back in.</span></span> <span data-ttu-id="03b7c-113">Se il problema persiste, aprire un ticket di supporto e sollevarlo come problema.</span><span class="sxs-lookup"><span data-stu-id="03b7c-113">If the problem persists, open a support ticket and raise this as an issue.</span></span> <span data-ttu-id="03b7c-114">Se si utilizza il ruolo di amministratore di Exchange per accedere al centro sicurezza e conformità, vedere il passaggio successivo.</span><span class="sxs-lookup"><span data-stu-id="03b7c-114">If you are using your Exchange Administrator role to access the Security and Compliance Center, see the next step.</span></span>
4. <span data-ttu-id="03b7c-115">Se si sta attivando un ruolo per accedere al centro sicurezza e conformità o se si sta attivando il ruolo di amministratore di SharePoint, si verificherà un ritardo di attivazione di alcuni minuti fino a poche ore.</span><span class="sxs-lookup"><span data-stu-id="03b7c-115">If you are activating a role to access the Security and Compliance Center or if you are activating the SharePoint Administrator role, you will experience some activation delay from a few minutes up to a few hours.</span></span> <span data-ttu-id="03b7c-116">Si tratta di un problema noto e stiamo lavorando attivamente con questi team per risolvere il problema nel più breve tempo possibile.</span><span class="sxs-lookup"><span data-stu-id="03b7c-116">This is a known issue and we are actively working with these teams to resolve this issue as soon as possible.</span></span>

<span data-ttu-id="03b7c-117">Per ulteriori informazioni, vedere:</span><span class="sxs-lookup"><span data-stu-id="03b7c-117">For more information, see:</span></span>

- [<span data-ttu-id="03b7c-118">Attivare i ruoli di Azure AD in PIM</span><span class="sxs-lookup"><span data-stu-id="03b7c-118">Activate my Azure AD roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [<span data-ttu-id="03b7c-119">Attivare i ruoli delle risorse di Azure in PIM</span><span class="sxs-lookup"><span data-stu-id="03b7c-119">Activate my Azure resource roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

<span data-ttu-id="03b7c-120">**Le autorizzazioni non vengono rimosse dopo la disattivazione di un ruolo o la scadenza dell'attivazione del ruolo**</span><span class="sxs-lookup"><span data-stu-id="03b7c-120">**Permissions are not removed after deactivating a role or the role activation expires**</span></span>

<span data-ttu-id="03b7c-121">Quando si disattiva un ruolo in Azure AD Privileged Identity Management o quando il periodo di attivazione di un ruolo scade, potrebbe verificarsi un ritardo in cui si continuerà a essere in grado di accedere.</span><span class="sxs-lookup"><span data-stu-id="03b7c-121">When you deactivate a role in Azure AD Privileged Identity Management or when a role activation period expires, there might be a delay where you continue to have access.</span></span>

<span data-ttu-id="03b7c-122">Se la disattivazione è in ritardo, procedere come segue:</span><span class="sxs-lookup"><span data-stu-id="03b7c-122">If your deactivation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="03b7c-123">Se si disattiva il ruolo di amministratore di Exchange o il periodo di attivazione del ruolo scade e si nota un ritardo significativo prima della rimozione delle autorizzazioni, aprire un ticket di supporto e informare il tecnico del supporto per l'archiviazione di un ticket con il team di gestione degli accessi con privilegi (PAM) in Office su questo problema.</span><span class="sxs-lookup"><span data-stu-id="03b7c-123">If you are deactivating the Exchange Administrator role or the role activation period expires, and you notice a significant delay before the permissions are removed, open a support ticket and tell your support engineer to help you file a ticket with the Privileged Access Management (PAM) team inside Office about this issue.</span></span>
2. <span data-ttu-id="03b7c-124">Se il periodo di attivazione è scaduto, ma la sessione del browser è ancora aperta, chiudere il browser.</span><span class="sxs-lookup"><span data-stu-id="03b7c-124">If the activation period has expired, but you still have the browser session open, close your browser.</span></span> <span data-ttu-id="03b7c-125">È possibile continuare a utilizzare il ruolo fino a quando non viene chiusa la sessione.</span><span class="sxs-lookup"><span data-stu-id="03b7c-125">You can continue to use the role until you close that session.</span></span> <span data-ttu-id="03b7c-126">Si tratta di un problema noto e si tratta di una possibile soluzione che consente di revocare attivamente ogni sessione una volta scaduta l'attivazione.</span><span class="sxs-lookup"><span data-stu-id="03b7c-126">This is a known issue and we are looking at a potential fix to actively revoke each session once activation has expired.</span></span>

<span data-ttu-id="03b7c-127">Se il ritardo è diverso rispetto a questi due scenari, aprire un ticket di supporto.</span><span class="sxs-lookup"><span data-stu-id="03b7c-127">If your delay is different than these two scenarios, please open a support ticket.</span></span>
