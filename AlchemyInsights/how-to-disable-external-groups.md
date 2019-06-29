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
ms.openlocfilehash: 95e60599b5298090db23bf887cb860350280964f
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/28/2019
ms.locfileid: "35384829"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="e6e39-102">Come disabilitare i gruppi esterni</span><span class="sxs-lookup"><span data-stu-id="e6e39-102">How to disable External Groups</span></span>

<span data-ttu-id="e6e39-103">La messaggistica esterna di Yammer applica le regole di trasporto di Exchange (ETRs), un insieme di controlli proattivi che impediscono la condivisione delle informazioni aziendali.</span><span class="sxs-lookup"><span data-stu-id="e6e39-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="e6e39-104">Per impedire agli utenti di creare gruppi esterni, è necessario configurare una regola di trasporto di Exchange (ETR), quindi configurare Yammer in modo da utilizzare la regola di trasporto di Exchange per bloccare la messaggistica esterna.</span><span class="sxs-lookup"><span data-stu-id="e6e39-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="e6e39-105">Dopo aver creato una regola nell'interfaccia di amministrazione di Exchange Online, eseguire la procedura seguente per impostare ETR per l'applicazione in Yammer:</span><span class="sxs-lookup"><span data-stu-id="e6e39-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="e6e39-106">Accedere a Yammer come amministratore verificato e, nell'interfaccia di **amministrazione di Yammer**, passare a impostazioni di \*\* \> sicurezza di contenuto e\*\* sicurezza di C.</span><span class="sxs-lookup"><span data-stu-id="e6e39-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="e6e39-107">In **messaggi esterni**selezionare **applica le regole di trasporto di Exchange Online (ETRs) in Yammer.**</span><span class="sxs-lookup"><span data-stu-id="e6e39-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="e6e39-108">Fare clic su **Salva**.</span><span class="sxs-lookup"><span data-stu-id="e6e39-108">Choose **Save**.</span></span>

<span data-ttu-id="e6e39-109">Per ulteriori informazioni, vedere [controllare la messaggistica esterna in una rete di Yammer con le regole di trasporto di Exchange](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span><span class="sxs-lookup"><span data-stu-id="e6e39-109">For more information, see [Control external messaging in a Yammer network with Exchange Transport rules](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span></span>
  