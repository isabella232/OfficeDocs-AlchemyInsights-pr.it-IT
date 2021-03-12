---
title: Set di repliche
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
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 3834696ff59b7e96e90a5b660a489003dfa9729c
ms.sourcegitcommit: 581c696ec108184adae9d4bc8f47cb9247131de8
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/10/2021
ms.locfileid: "50716272"
---
# <a name="replica-set"></a><span data-ttu-id="159b3-102">Set di repliche</span><span class="sxs-lookup"><span data-stu-id="159b3-102">Replica set</span></span>

<span data-ttu-id="159b3-103">AADDS viene chiamato anche come dominio gestito.</span><span class="sxs-lookup"><span data-stu-id="159b3-103">AADDS is also called as the managed domain.</span></span> <span data-ttu-id="159b3-104">Si tratta in realtà di due controller di dominio eseguiti e gestiti dal back-end.</span><span class="sxs-lookup"><span data-stu-id="159b3-104">It is actually two domain controllers that are run and maintained by the backend.</span></span> <span data-ttu-id="159b3-105">I due controller di dominio includono un controller di dominio principale e un controller di dominio di replica.</span><span class="sxs-lookup"><span data-stu-id="159b3-105">The two DCs include one main DC and one replication DC.</span></span> <span data-ttu-id="159b3-106">I backup in AADDS (dominio gestito) sono processi automatizzati gestiti dalla piattaforma Azure.</span><span class="sxs-lookup"><span data-stu-id="159b3-106">Backups in AADDS (managed domain) are an automated process managed by the Azure platform.</span></span> <span data-ttu-id="159b3-107">In caso di un problema con il dominio gestito, il supporto di Azure può essere di aiuto nel ripristino dal backup.</span><span class="sxs-lookup"><span data-stu-id="159b3-107">In the event of an issue with your managed domain, Azure support can assist you in restoring from backup.</span></span>

<span data-ttu-id="159b3-108">Ogni set di repliche viene creato in una rete virtuale.</span><span class="sxs-lookup"><span data-stu-id="159b3-108">You create each replica set in a virtual network.</span></span> <span data-ttu-id="159b3-109">Ogni rete virtuale deve essere peered a ogni altra rete virtuale che ospita il set di repliche di un dominio gestito.</span><span class="sxs-lookup"><span data-stu-id="159b3-109">Each virtual network must be peered to every other virtual network that hosts a managed domain's replica set.</span></span> <span data-ttu-id="159b3-110">Questa configurazione crea una topologia di rete mesh che supporta la replica della directory.</span><span class="sxs-lookup"><span data-stu-id="159b3-110">This configuration creates a mesh network topology that supports directory replication.</span></span> <span data-ttu-id="159b3-111">Una rete virtuale può supportare più set di repliche, purché ogni set di repliche si trova in una subnet virtuale diversa.</span><span class="sxs-lookup"><span data-stu-id="159b3-111">A virtual network can support multiple replica sets, provided that each replica set is in a different virtual subnet.</span></span>

<span data-ttu-id="159b3-112">Per ulteriori informazioni sul set di repliche, vedere [Concepts Replica sets.](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets)</span><span class="sxs-lookup"><span data-stu-id="159b3-112">For more details on Replica set, see [Concepts Replica sets](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).</span></span>
