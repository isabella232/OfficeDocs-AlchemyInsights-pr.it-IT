---
title: Configurare il servizio di dominio
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7931"
- "9004400"
ms.openlocfilehash: 51e0bd78240627876721cbce654188afac1ee365
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884591"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a><span data-ttu-id="1f1de-102">Impossibile abilitare AAD-DS o errore restituito nell'ambito della distribuzione</span><span class="sxs-lookup"><span data-stu-id="1f1de-102">Unable to enable AAD-DS or deployment is failing</span></span>

<span data-ttu-id="1f1de-103">Per poter abilitare o distribuire Azure Active Directory Domain Services, seguire questi passaggi:</span><span class="sxs-lookup"><span data-stu-id="1f1de-103">To solve the issue of Azure AD domain service (AAD-DS) not being enabled or failing to be deployed, perform the following steps:</span></span>

1. <span data-ttu-id="1f1de-104">Se si sta usando una rete virtuale già esistente, controllare il gruppo di sicurezza di rete per rilevare eventuali regole che bloccano le porte necessarie per la sincronizzazione in AAD-DS nel portale https://aka.ms/aadds-networking.</span><span class="sxs-lookup"><span data-stu-id="1f1de-104">If you are using an already existing virtual network, check your NSG for rules that block ports needed to synchronize in AAD-DS in the portal https://aka.ms/aadds-networking.</span></span>
2. <span data-ttu-id="1f1de-105">Controllare se è presente la risposta al messaggio di errore nella guida disponibile in  https://aka.ms/aadds-troubleshoot-enable.</span><span class="sxs-lookup"><span data-stu-id="1f1de-105">Check to see if your error message is answered in this troubleshooting guide that is available in  https://aka.ms/aadds-troubleshoot-enable.</span></span>
3. <span data-ttu-id="1f1de-106">Provare a distribuire Azure Active Directory Domain Services in una nuova rete virtuale.</span><span class="sxs-lookup"><span data-stu-id="1f1de-106">Try deploying Azure AD Domain Services in a new virtual network.</span></span>
4. <span data-ttu-id="1f1de-107">Seguire la Guida introduttiva su come distribuire AAD-DS: [Creare e configurare Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span><span class="sxs-lookup"><span data-stu-id="1f1de-107">Follow the Getting Started guide on how to deploy AAD-DS: [Create and Configure AAD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span></span>
5. <span data-ttu-id="1f1de-108">In caso di problemi con la distribuzione di Azure Active Directory Domain Services, vedere [Risolvere i problemi di Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) per risolvere gli errori comuni e ripristinare il servizio.</span><span class="sxs-lookup"><span data-stu-id="1f1de-108">If you are having issues with Deploying Azure AD Domain Services, see [Troubleshoot Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) to resolve common errors to help you get things working again.</span></span> 

<span data-ttu-id="1f1de-109">**Impossibile disabilitare AAD-DS**</span><span class="sxs-lookup"><span data-stu-id="1f1de-109">**Unable to disable AAD-DS**</span></span>

<span data-ttu-id="1f1de-110">AAD-DS non può essere messo in pausa.</span><span class="sxs-lookup"><span data-stu-id="1f1de-110">AAD-DS is unable to be paused.</span></span> <span data-ttu-id="1f1de-111">Per interrompere l'utilizzo del dominio gestito è necessario eliminarlo.</span><span class="sxs-lookup"><span data-stu-id="1f1de-111">If you wish to stop using your managed domain, it must be deleted.</span></span>
<span data-ttu-id="1f1de-112">Per eliminare il dominio gestito, vedere [Eliminare Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).</span><span class="sxs-lookup"><span data-stu-id="1f1de-112">To delete your Managed domain, see [Delete AAD Domain Service](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).</span></span>



