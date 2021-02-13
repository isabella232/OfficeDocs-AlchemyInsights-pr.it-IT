---
title: Problemi con i gruppi di sicurezza
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8252"
- "9004397"
ms.openlocfilehash: 1198b79c3301bd2752a7385a6ba6746c8f0c2b5b
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162944"
---
# <a name="issue-with-security-groups"></a><span data-ttu-id="8e583-102">Problemi con i gruppi di sicurezza</span><span class="sxs-lookup"><span data-stu-id="8e583-102">Issue with security groups</span></span>

<span data-ttu-id="8e583-103">**Se si riceve un errore di rete AADDS104**</span><span class="sxs-lookup"><span data-stu-id="8e583-103">**If you are getting Network Error AADDS104**</span></span>

<span data-ttu-id="8e583-104">Le regole non valide dei gruppi di sicurezza di rete sono la causa più comune degli errori di rete per Servizi di dominio Azure Active Directory (AD DS).</span><span class="sxs-lookup"><span data-stu-id="8e583-104">Invalid network security group rules are the most common cause of network errors for Azure Active Directory Domain Services (AD DS).</span></span> <span data-ttu-id="8e583-105">Il gruppo di sicurezza di rete per la rete virtuale deve consentire l'accesso a porte e protocolli specifici.</span><span class="sxs-lookup"><span data-stu-id="8e583-105">The network security group for the virtual network must allow access to specific ports and protocols.</span></span> <span data-ttu-id="8e583-106">Se queste porte sono bloccate, la piattaforma Azure non può monitorare o aggiornare il dominio gestito.</span><span class="sxs-lookup"><span data-stu-id="8e583-106">If these ports are blocked, the Azure platform can't monitor or update the managed domain.</span></span> <span data-ttu-id="8e583-107">Ha anche effetto sulla sincronizzazione tra Azure AD e Azure AD DS.</span><span class="sxs-lookup"><span data-stu-id="8e583-107">The synchronization between the Azure AD and Azure AD DS is also impacted.</span></span> <span data-ttu-id="8e583-108">Assicurarsi di tenere aperte le porte predefinite per evitare interruzioni del servizio.</span><span class="sxs-lookup"><span data-stu-id="8e583-108">Ensure you keep the default ports open to avoid interruption in service.</span></span>

<span data-ttu-id="8e583-109">Per comprendere e risolvere gli avvisi comuni per i problemi di configurazione dei gruppi di sicurezza di rete, vedere [Aggiungere e verificare i gruppi di sicurezza](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).</span><span class="sxs-lookup"><span data-stu-id="8e583-109">To understand and to resolve common alerts for network security group configuration issues, see [Add and Verify Security Groups](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).</span></span>
