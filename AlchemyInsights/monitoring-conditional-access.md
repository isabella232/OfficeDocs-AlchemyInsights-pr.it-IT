---
title: Monitoraggio dell'accesso condizionale
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 756c5e98ed3e9cedd0152b5747ea6bf1ed31778e
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32418473"
---
# <a name="monitoring-conditional-access"></a><span data-ttu-id="027f1-102">Monitoraggio dell'accesso condizionale</span><span class="sxs-lookup"><span data-stu-id="027f1-102">Monitoring Conditional Access</span></span>

<span data-ttu-id="027f1-103">Gli utenti a cui viene assegnato l'accesso condizionale ricevono un messaggio di posta elettronica di notifica se non soddisfano i requisiti di accesso dell'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="027f1-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="027f1-104">Per risolvere il testo, è consigliabile eseguire una o più delle soluzioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="027f1-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="027f1-105">Se si presume che il dispositivo venga registrato, avvisare l'utente di accedere all'app portale aziendale e verificare che venga visualizzato nel portale aziendale.</span><span class="sxs-lookup"><span data-stu-id="027f1-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="027f1-106">In caso contrario, l'utente deve registrare il dispositivo.</span><span class="sxs-lookup"><span data-stu-id="027f1-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="027f1-107">Nel portale di Azure passare a **Intune \> Device Compliance**.</span><span class="sxs-lookup"><span data-stu-id="027f1-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="027f1-108">In **Monitor** fare clic su **conformità dispositivo**.</span><span class="sxs-lookup"><span data-stu-id="027f1-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="027f1-109">Visualizzare il rapporto di conformità del dispositivo per verificare che il dispositivo dell'utente sia contrassegnato come conforme.</span><span class="sxs-lookup"><span data-stu-id="027f1-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="027f1-110">Nel portale di Azure passare a **Intune \> Device Compliance**.</span><span class="sxs-lookup"><span data-stu-id="027f1-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="027f1-111">In **Gestisci**fare clic su **criteri**.</span><span class="sxs-lookup"><span data-stu-id="027f1-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="027f1-112">Nell'elenco dei criteri di conformità, verificare che un profilo sia assegnato al dispositivo dell'utente.</span><span class="sxs-lookup"><span data-stu-id="027f1-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="027f1-113">Se non è stato assegnato alcun profilo, Intune non sarà in grado di confermare lo stato di conformità del dispositivo.</span><span class="sxs-lookup"><span data-stu-id="027f1-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="027f1-114">Modificare l'assegnazione di accesso condizionale dell'utente.</span><span class="sxs-lookup"><span data-stu-id="027f1-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="027f1-115">Nel portale di Azure passare ai **criteri \> di accesso \> condizionale di Intune**</span><span class="sxs-lookup"><span data-stu-id="027f1-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="027f1-116">Selezionare un criterio dall'elenco</span><span class="sxs-lookup"><span data-stu-id="027f1-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="027f1-117">Fare clic su **utenti e gruppi**</span><span class="sxs-lookup"><span data-stu-id="027f1-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="027f1-118">Per assegnare un determinato criterio a un utente, aggiungerli all' \*\*\*\* elenco Includi.</span><span class="sxs-lookup"><span data-stu-id="027f1-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="027f1-119">Per assicurarsi che una persona venga omessa dal criterio, aggiungerla all'elenco **Escludi** .</span><span class="sxs-lookup"><span data-stu-id="027f1-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="027f1-120">Per ulteriori informazioni [, vedere: come monitorare i dispositivi di accesso condizionale](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="027f1-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

