---
title: Problema con un singolo utente
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8469"
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/04/2021
ms.locfileid: "50428830"
---
# <a name="problem-with-single-user"></a><span data-ttu-id="098b3-102">Problema con un singolo utente</span><span class="sxs-lookup"><span data-stu-id="098b3-102">Problem with single user</span></span>

- <span data-ttu-id="098b3-103">Il provisioning dell'utente potrebbe non essere stato eseguito perché il servizio non ha ancora avuto la possibilità di valutare l'utente.</span><span class="sxs-lookup"><span data-stu-id="098b3-103">The user may not have been provisioned because the service hasn't had a chance to evaluate the user yet.</span></span> <span data-ttu-id="098b3-104">Esaminare le indicazioni relative al tempo necessario per il provisioning e la barra di avanzamento nella pagina di configurazione del provisioning.</span><span class="sxs-lookup"><span data-stu-id="098b3-104">Review the guidance for how long provisioning takes as well as the progress bar on the provisioning configuration page.</span></span> <span data-ttu-id="098b3-105">Se lo stato stabile specificato nella sezione dei dettagli aggiuntivi è precedente alla data di creazione/aggiornamento/eliminazione dell'utente, significa che non è stato ancora valutato l'utente.</span><span class="sxs-lookup"><span data-stu-id="098b3-105">If the steady state specified in the additional details section is before the date the user was created/updated/deleted, it means we have not evaluated the user yet.</span></span> <span data-ttu-id="098b3-106">In questo scenario, la cosa migliore da fare è attendere il completamento del servizio di provisioning.</span><span class="sxs-lookup"><span data-stu-id="098b3-106">In this scenario, the best thing to do is wait for the provisioning service to finish.</span></span>

  - <span data-ttu-id="098b3-107">Tieni presente che il servizio è a conoscenza solo delle modifiche apportate a un utente nel sistema di origine (Cloud HR).</span><span class="sxs-lookup"><span data-stu-id="098b3-107">Note that our service is only aware of changes to a user in the source system (Cloud HR).</span></span> <span data-ttu-id="098b3-108">Deve essere presente una modifica valida nel sistema di origine in modo che Azure AD rilevi la modifica e la trasla in Active Directory.</span><span class="sxs-lookup"><span data-stu-id="098b3-108">There has to be a valid change in the source system for Azure AD to detect the change and flow it into Active Directory.</span></span>
- <span data-ttu-id="098b3-109">Il servizio di provisioning ha valutato l'utente e ha determinato che non deve essere effettuato il provisioning:</span><span class="sxs-lookup"><span data-stu-id="098b3-109">Provisioning service evaluated the user and determined it should not be provisioned:</span></span>
  - <span data-ttu-id="098b3-110">Se è stato impostato un filtro di ambito basato su attributi, verificare che l'utente soddisfi i criteri specificati.</span><span class="sxs-lookup"><span data-stu-id="098b3-110">If you have set an attribute based scoping filter, ensure that the user meets the criteria that you have specified.</span></span>
  - <span data-ttu-id="098b3-111">Se gli utenti esistono già nel sistema di destinazione e lo stato dell'utente nella corrispondenza di origine e destinazione, non eseguiremo ulteriori azioni.</span><span class="sxs-lookup"><span data-stu-id="098b3-111">If users already exist in the target system and the state of the user in the source and target match, we won't take any further action.</span></span>
- <span data-ttu-id="098b3-112">Il servizio di provisioning ha tentato di eseguire il provisioning dell'utente e non è riuscito.</span><span class="sxs-lookup"><span data-stu-id="098b3-112">Provisioning service attempted to provision the user and it failed.</span></span> <span data-ttu-id="098b3-113">Per questi scenari, esaminare la scheda per la risoluzione dei problemi e gli elementi consigliati dei log di provisioning:</span><span class="sxs-lookup"><span data-stu-id="098b3-113">For these scenarios, review the troubleshooting and recommendations tab of the provisioning logs:</span></span>
  - <span data-ttu-id="098b3-114">Un attributo obbligatorio per l'utente potrebbe non essere presente in Active Directory locale o Azure AD.</span><span class="sxs-lookup"><span data-stu-id="098b3-114">A required attribute on the user might be missing in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="098b3-115">Ad esempio, le regole di generazione userPrincipalName o sAMAccountName non generano il valore giusto.</span><span class="sxs-lookup"><span data-stu-id="098b3-115">For example, the userPrincipalName or sAMAccountName generation rules are not generating the right value.</span></span>
  - <span data-ttu-id="098b3-116">L'attributo corrispondente (in genere employeeId) non risolve un utente univoco in Active Directory locale o Azure AD.</span><span class="sxs-lookup"><span data-stu-id="098b3-116">The matching attribute (usually employeeId) is not resolving to a unique user in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="098b3-117">Ad esempio, ci sono due utenti con lo stesso employeeId in Active Directory e il servizio restituisce un codice di errore che indica voci di destinazione duplicate per la stessa voce di origine.</span><span class="sxs-lookup"><span data-stu-id="098b3-117">For example, there are two users with the same employeeId in AD and the service returns an error code indicate duplicate target entries for the same source entry.</span></span>

<span data-ttu-id="098b3-118">Per esaminare i log per singoli utenti e gruppi, vedere [Esaminare i log di provisioning per un problema con un utente specifico.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs)</span><span class="sxs-lookup"><span data-stu-id="098b3-118">To review logs for single user and groups, see [Review the provisioning logs for an issue with a specific user](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).</span></span>
