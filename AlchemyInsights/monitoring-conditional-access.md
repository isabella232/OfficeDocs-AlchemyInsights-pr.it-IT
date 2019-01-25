---
title: Monitoraggio accesso condizionale
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 06307b57475e8828e6d4e5e01625d5100576f12b
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/24/2019
ms.locfileid: "29475399"
---
# <a name="monitoring-conditional-access"></a><span data-ttu-id="cbaf7-102">Monitoraggio accesso condizionale</span><span class="sxs-lookup"><span data-stu-id="cbaf7-102">Monitoring Conditional Access</span></span>

<span data-ttu-id="cbaf7-p101">Se non soddisfano i requisiti dell'organizzazione access, gli utenti assegnati con accesso condizionale riceveranno un messaggio di posta elettronica di notifica. Per risolvere, è consigliabile una o più delle soluzioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="cbaf7-p101">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements. To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="cbaf7-p102">Se il dispositivo presumendo che iscritto, consigliare all'utente di accedere all'applicazione portale della società e verificare che venga visualizzato nel portale della società. In caso contrario, l'utente deve registrare il dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cbaf7-p102">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal. If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="cbaf7-p103">Nel portale di Azure passare a **Intune \> conformità dispositivo**. In **Monitor** fare clic su **dispositivo conformità**. Visualizzare il report di conformità di dispositivo per verificare che il dispositivo dell'utente è contrassegnato come compatibile.</span><span class="sxs-lookup"><span data-stu-id="cbaf7-p103">In the Azure portal go to **Intune \> Device compliance**. Under **Monitor** click **Device compliance**. View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="cbaf7-p104">Nel portale di Azure passare a **Intune \> conformità dispositivo**. In **Gestione**fare clic su **criteri**. Nell'elenco dei criteri di conformità, verificare che un profilo viene assegnato al dispositivo dell'utente. Se non viene assegnato alcun profilo, Intune non sarà in grado di verificare lo stato della conformità del dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cbaf7-p104">In the Azure portal go to **Intune \> Device compliance**. Under **Manage**, click **Policies**. In the list of compliance policies, verify that a profile is assigned to your user's device. If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="cbaf7-114">Modificare l'assegnazione di accesso condizionato dell'utente.</span><span class="sxs-lookup"><span data-stu-id="cbaf7-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="cbaf7-115">Nel portale di Azure passare a **Intune \> accesso condizionato \> criteri**</span><span class="sxs-lookup"><span data-stu-id="cbaf7-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="cbaf7-116">Selezionare un criterio nell'elenco</span><span class="sxs-lookup"><span data-stu-id="cbaf7-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="cbaf7-117">Fare clic su **utenti e gruppi**</span><span class="sxs-lookup"><span data-stu-id="cbaf7-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="cbaf7-p105">Per un determinato criterio a un utente di destinazione, aggiungerli all'elenco di **inclusione** . Per garantire che un utente viene omesso il parametro dal criterio, aggiungerli all'elenco di **esclusione** .</span><span class="sxs-lookup"><span data-stu-id="cbaf7-p105">To target a certain policy at someone, add them to the **Include** list. To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="cbaf7-120">Ulteriori: [come monitorare gli accessi condizionale dispositivi](https://docs.microsoft.com/en-us/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="cbaf7-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/en-us/intune/conditional-access-exchange-monitor)</span></span>
  

