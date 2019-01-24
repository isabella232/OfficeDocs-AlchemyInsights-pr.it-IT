---
title: Come disabilitare gruppi esterni
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 4807dbfbabcea1f13785bd39bb48e4bbaa8d0f0f
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/24/2019
ms.locfileid: "29476244"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="b4068-102">Come disabilitare gruppi esterni</span><span class="sxs-lookup"><span data-stu-id="b4068-102">How to disable External Groups</span></span>

<span data-ttu-id="b4068-p101">Yammer messaggistica esterni si applica regole di trasporto Exchange (ETRs), un insieme di controlli proattivi per impedire che informazioni società condiviso. Per impedire agli utenti di creare gruppi esterni, è necessario configurare una regola di trasporto di Exchange (ETR) e quindi configurare Yammer per l'utilizzo della regola di trasporto di Exchange per bloccare la messaggistica esterno.</span><span class="sxs-lookup"><span data-stu-id="b4068-p101">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared. In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span> 
  
<span data-ttu-id="b4068-105">Dopo aver creato una regola nell'interfaccia di amministrazione di Exchange Online, eseguire la procedura seguente per impostare ETR da applicare in Yammer:</span><span class="sxs-lookup"><span data-stu-id="b4068-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="b4068-106">Accedere a Yammer come un amministratore verificato e nell' **interfaccia di amministrazione di Yammer**, andare alla C **obbligatoria e sicurezza \> le impostazioni di sicurezza.**</span><span class="sxs-lookup"><span data-stu-id="b4068-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **ontent and Security \> Security Settings.**</span></span>
    
- <span data-ttu-id="b4068-107">In **Messaggistica esterno**, selezionare **applicare i Exchange Transport Rules Exchange Online (ETRs) in Yammer.**</span><span class="sxs-lookup"><span data-stu-id="b4068-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>
    
- <span data-ttu-id="b4068-108">Scegliere **Save**.</span><span class="sxs-lookup"><span data-stu-id="b4068-108">Choose **Save**.</span></span> 
    
<span data-ttu-id="b4068-109">Per ulteriori informazioni, vedere [controllo esterno messaggistica in una rete Yammer con le regole di trasporto di Exchange](https://support.office.com/en-us/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span><span class="sxs-lookup"><span data-stu-id="b4068-109">For more information, see [Control external messaging in a Yammer network with Exchange Transport rules](https://support.office.com/en-us/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span></span>
  

