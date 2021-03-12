---
title: Monitoraggio dell'accesso condizionale
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: c3bf5dd9066685af2df7ba50f0eb3ba6e891c2a9
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708678"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="352fd-102">Monitoraggio dell'accesso condizionale per Exchange</span><span class="sxs-lookup"><span data-stu-id="352fd-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="352fd-103">Gli utenti con accesso condizionale riceveranno un messaggio di posta elettronica di notifica se non soddisfano i requisiti di accesso dell'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="352fd-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="352fd-104">Per risolvere il problema, è consigliabile utilizzare una o più delle soluzioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="352fd-104">To resolve, we recommend one or more of the following solutions:</span></span>

- <span data-ttu-id="352fd-105">Se si presume che il dispositivo sia registrato, consigliare all'utente di passare all'app Portale aziendale e verificare che venga visualizzato nel portale aziendale.</span><span class="sxs-lookup"><span data-stu-id="352fd-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="352fd-106">In caso contrario, l'utente deve registrare il dispositivo.</span><span class="sxs-lookup"><span data-stu-id="352fd-106">If it doesn't, the user should enroll the device.</span></span>
- <span data-ttu-id="352fd-107">Nel portale di Azure passare a Intune > conformità del dispositivo.</span><span class="sxs-lookup"><span data-stu-id="352fd-107">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="352fd-108">In Monitoraggio fare clic su Conformità dispositivo.</span><span class="sxs-lookup"><span data-stu-id="352fd-108">Under Monitor click Device compliance.</span></span> <span data-ttu-id="352fd-109">Visualizzare il report di conformità del dispositivo per verificare che il dispositivo dell'utente sia contrassegnato come conforme.</span><span class="sxs-lookup"><span data-stu-id="352fd-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span>
- <span data-ttu-id="352fd-110">Nel portale di Azure passare a Intune > conformità del dispositivo.</span><span class="sxs-lookup"><span data-stu-id="352fd-110">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="352fd-111">In Gestisci fare clic su Criteri.</span><span class="sxs-lookup"><span data-stu-id="352fd-111">Under Manage, click Policies.</span></span> <span data-ttu-id="352fd-112">Nell'elenco dei criteri di conformità, verificare che un profilo sia assegnato al dispositivo dell'utente.</span><span class="sxs-lookup"><span data-stu-id="352fd-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="352fd-113">Se non viene assegnato alcun profilo, Intune non sarà in grado di confermare lo stato di conformità del dispositivo.</span><span class="sxs-lookup"><span data-stu-id="352fd-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
- <span data-ttu-id="352fd-114">Modificare l'assegnazione di accesso condizionale dell'utente.</span><span class="sxs-lookup"><span data-stu-id="352fd-114">Edit the user's conditional access assignment.</span></span>

1. <span data-ttu-id="352fd-115">Nel portale di Azure passare a **Criteri di accesso** condizionale  >  **di**  >  Intune.</span><span class="sxs-lookup"><span data-stu-id="352fd-115">In the Azure portal go to **Intune** > **Conditional access** > **Policies**.</span></span>
2. <span data-ttu-id="352fd-116">Selezionare un criterio dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="352fd-116">Select a policy from the list.</span></span>
3. <span data-ttu-id="352fd-117">Fare clic su Utenti e gruppi.</span><span class="sxs-lookup"><span data-stu-id="352fd-117">Click Users and groups.</span></span>
4. <span data-ttu-id="352fd-118">Per impostare come destinazione un determinato criterio presso un utente, aggiungerlo all'elenco Includi.</span><span class="sxs-lookup"><span data-stu-id="352fd-118">To target a certain policy at someone, add them to the Include list.</span></span> <span data-ttu-id="352fd-119">Per assicurarsi che una persona sia omessa dal criterio, aggiungerla all'elenco Escludi.</span><span class="sxs-lookup"><span data-stu-id="352fd-119">To ensure that a person is omitted from the policy, add them to the Exclude list.</span></span>

<span data-ttu-id="352fd-120">Collegamenti utili:</span><span class="sxs-lookup"><span data-stu-id="352fd-120">Helpful links:</span></span>

[<span data-ttu-id="352fd-121">Panoramica della conformità dei dispositivi</span><span class="sxs-lookup"><span data-stu-id="352fd-121">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="352fd-122">Risoluzione dei problemi dell'autorità di certificazione</span><span class="sxs-lookup"><span data-stu-id="352fd-122">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="352fd-123">Criteri per la risoluzione dei problemi</span><span class="sxs-lookup"><span data-stu-id="352fd-123">Troubleshooting policy</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[<span data-ttu-id="352fd-124">Monitoraggio della conformità dei dispositivi Intune</span><span class="sxs-lookup"><span data-stu-id="352fd-124">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

<span data-ttu-id="352fd-125">Nota: questi passaggi sono utili solo per la risoluzione dei problemi relativi alla funzionalità accesso condizionale di Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="352fd-125">Note: these steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="352fd-126">È anche possibile mettere in quarantena un dispositivo che blocca l'accesso alla posta elettronica con i criteri di Exchange.</span><span class="sxs-lookup"><span data-stu-id="352fd-126">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="352fd-127">Ulteriori informazioni sulla gestione dei dispositivi di Exchange sono disponibili [qui]( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .</span><span class="sxs-lookup"><span data-stu-id="352fd-127">More information on Exchange device management can be found [here](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141).</span></span>
