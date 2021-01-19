---
title: 'Controller di dominio '
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7909"
- "9003233"
ms.openlocfilehash: d4cbe80c3e8f0ce32fcbe89e852f24efd6f50575
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 01/18/2021
ms.locfileid: "49886848"
---
# <a name="domain-controller"></a><span data-ttu-id="bef49-102">Controller di dominio</span><span class="sxs-lookup"><span data-stu-id="bef49-102">Domain controller</span></span>

<span data-ttu-id="bef49-103">**Impossibile abilitare AAD-DS o errore restituito nell'ambito della distribuzione**</span><span class="sxs-lookup"><span data-stu-id="bef49-103">**Unable to enable AAD-DS or deployment is failing**</span></span>

<span data-ttu-id="bef49-104">Per poter abilitare o distribuire Azure Active Directory Domain Services, seguire questi passaggi:</span><span class="sxs-lookup"><span data-stu-id="bef49-104">To solve the issue of Azure AD domain service (AAD-DS) not being enabled or failing to be deployed, perform the following steps:</span></span>

1. <span data-ttu-id="bef49-105">Se si sta usando una rete virtuale già esistente, controllare il gruppo di sicurezza di rete per rilevare eventuali regole che bloccano le porte necessarie per la sincronizzazione in AAD-DS nel portale https://aka.ms/aadds-networking.</span><span class="sxs-lookup"><span data-stu-id="bef49-105">If you are using an already existing virtual network, check your NSG for rules that block ports needed to synchronize in AAD-DS in the portal https://aka.ms/aadds-networking.</span></span>
2. <span data-ttu-id="bef49-106">Controllare se è presente la risposta al messaggio di errore nella guida disponibile in  https://aka.ms/aadds-troubleshoot-enable.</span><span class="sxs-lookup"><span data-stu-id="bef49-106">Check to see if your error message is answered in this troubleshooting guide that is available in  https://aka.ms/aadds-troubleshoot-enable.</span></span>
3. <span data-ttu-id="bef49-107">Provare a distribuire Azure Active Directory Domain Services in una nuova rete virtuale.</span><span class="sxs-lookup"><span data-stu-id="bef49-107">Try deploying Azure AD Domain Services in a new virtual network.</span></span>
4. <span data-ttu-id="bef49-108">Seguire la Guida introduttiva su come distribuire AAD-DS, disponibile qui [Tutorial per creare Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span><span class="sxs-lookup"><span data-stu-id="bef49-108">Follow the Getting Started guide on how to deploy AAD-DS, which is available at [Tutorial to Create Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span></span>
5. <span data-ttu-id="bef49-109">In caso di problemi con la distribuzione di Azure Active Directory Domain Services, vedere [Risolvere i problemi di Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) per risolvere gli errori comuni e ripristinare il servizio.</span><span class="sxs-lookup"><span data-stu-id="bef49-109">If you are having issues with Deploying Azure AD Domain Services, see [Troubleshoot Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) to resolve common errors to help you get things working again.</span></span> 

<span data-ttu-id="bef49-110">**Impossibile disabilitare AAD-DS**</span><span class="sxs-lookup"><span data-stu-id="bef49-110">**Unable to disable AAD-DS**</span></span>

<span data-ttu-id="bef49-111">AAD-DS non può essere messo in pausa.</span><span class="sxs-lookup"><span data-stu-id="bef49-111">AAD-DS is unable to be paused.</span></span> <span data-ttu-id="bef49-112">Per interrompere l'utilizzo del dominio gestito è necessario eliminarlo.</span><span class="sxs-lookup"><span data-stu-id="bef49-112">If you wish to stop using your managed domain, it must be deleted.</span></span>

<span data-ttu-id="bef49-113">Se si incorre in errori, per risolvere messaggi di errori comuni e i relativi passaggi per la risoluzione dei problemi e ripristinare il servizio, vedere [Risolvere i problemi di Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).</span><span class="sxs-lookup"><span data-stu-id="bef49-113">If you run into issues, to resolve common error messages and for associated troubleshooting steps to help you get things running again, see [Troubleshoot Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).</span></span>
