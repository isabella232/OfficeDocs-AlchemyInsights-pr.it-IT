---
title: Come disabilitare i gruppi esterni
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: b2328ea85d3ff6ec722cc56d8a46395d8438f79c
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 10/18/2019
ms.locfileid: "36739497"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="3eeb7-102">Come disabilitare i gruppi esterni</span><span class="sxs-lookup"><span data-stu-id="3eeb7-102">How to disable External Groups</span></span>

<span data-ttu-id="3eeb7-103">La messaggistica esterna di Yammer applica le regole di trasporto di Exchange (ETRs), un insieme di controlli proattivi che impediscono la condivisione delle informazioni aziendali.</span><span class="sxs-lookup"><span data-stu-id="3eeb7-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="3eeb7-104">Per impedire agli utenti di creare gruppi esterni, è necessario configurare una regola di trasporto di Exchange (ETR), quindi configurare Yammer in modo da utilizzare la regola di trasporto di Exchange per bloccare la messaggistica esterna.</span><span class="sxs-lookup"><span data-stu-id="3eeb7-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="3eeb7-105">Dopo aver creato una regola nell'interfaccia di amministrazione di Exchange Online, eseguire la procedura seguente per impostare ETR per l'applicazione in Yammer:</span><span class="sxs-lookup"><span data-stu-id="3eeb7-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="3eeb7-106">Accedere a Yammer come amministratore verificato e, nell'interfaccia di **amministrazione di Yammer**, passare a impostazioni di \*\* \> sicurezza di contenuto e\*\* sicurezza di C.</span><span class="sxs-lookup"><span data-stu-id="3eeb7-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="3eeb7-107">In **messaggi esterni**selezionare **applica le regole di trasporto di Exchange Online (ETRs) in Yammer.**</span><span class="sxs-lookup"><span data-stu-id="3eeb7-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="3eeb7-108">Fare clic su **Salva**.</span><span class="sxs-lookup"><span data-stu-id="3eeb7-108">Choose **Save**.</span></span>

<span data-ttu-id="3eeb7-109">Per ulteriori informazioni, vedere [Disable External Messaging in a Yammer Network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span><span class="sxs-lookup"><span data-stu-id="3eeb7-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  