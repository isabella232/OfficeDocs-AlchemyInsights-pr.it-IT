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
ms.openlocfilehash: 0687875a3714067e774872d02630564858d71d1b
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366432"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="5ce65-102">Monitoraggio dell'accesso condizionale per Exchange</span><span class="sxs-lookup"><span data-stu-id="5ce65-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="5ce65-103">Gli utenti a cui viene assegnato l'accesso condizionale ricevono un messaggio di posta elettronica di notifica se non soddisfano i requisiti di accesso dell'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="5ce65-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="5ce65-104">Per risolvere il testo, è consigliabile eseguire una o più delle soluzioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="5ce65-104">To resolve, we recommend one or more of the following solutions:</span></span>

- <span data-ttu-id="5ce65-105">Se si presume che il dispositivo venga registrato, avvisare l'utente di accedere all'app portale aziendale e verificare che venga visualizzato nel portale aziendale.</span><span class="sxs-lookup"><span data-stu-id="5ce65-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="5ce65-106">In caso contrario, l'utente deve registrare il dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5ce65-106">If it doesn't, the user should enroll the device.</span></span>
- <span data-ttu-id="5ce65-107">Nel portale di Azure passare a Intune > conformità del dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5ce65-107">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="5ce65-108">In Monitor fare clic su conformità dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5ce65-108">Under Monitor click Device compliance.</span></span> <span data-ttu-id="5ce65-109">Visualizzare il rapporto di conformità del dispositivo per verificare che il dispositivo dell'utente sia contrassegnato come conforme.</span><span class="sxs-lookup"><span data-stu-id="5ce65-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span>
- <span data-ttu-id="5ce65-110">Nel portale di Azure passare a Intune > conformità del dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5ce65-110">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="5ce65-111">In Gestisci fare clic su criteri.</span><span class="sxs-lookup"><span data-stu-id="5ce65-111">Under Manage, click Policies.</span></span> <span data-ttu-id="5ce65-112">Nell'elenco dei criteri di conformità, verificare che un profilo sia assegnato al dispositivo dell'utente.</span><span class="sxs-lookup"><span data-stu-id="5ce65-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="5ce65-113">Se non è stato assegnato alcun profilo, Intune non sarà in grado di confermare lo stato di conformità del dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5ce65-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
- <span data-ttu-id="5ce65-114">Modificare l'assegnazione di accesso condizionale dell'utente.</span><span class="sxs-lookup"><span data-stu-id="5ce65-114">Edit the user's conditional access assignment.</span></span>

1. <span data-ttu-id="5ce65-115">Nel portale di Azure passare ai **Intune**  >  criteri di**accesso condizionale**di Intune  >  **Policies**.</span><span class="sxs-lookup"><span data-stu-id="5ce65-115">In the Azure portal go to **Intune** > **Conditional access** > **Policies**.</span></span>
2. <span data-ttu-id="5ce65-116">Selezionare un criterio dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="5ce65-116">Select a policy from the list.</span></span>
3. <span data-ttu-id="5ce65-117">Fare clic su utenti e gruppi.</span><span class="sxs-lookup"><span data-stu-id="5ce65-117">Click Users and groups.</span></span>
4. <span data-ttu-id="5ce65-118">Per assegnare un determinato criterio a un utente, aggiungerli all'elenco Includi.</span><span class="sxs-lookup"><span data-stu-id="5ce65-118">To target a certain policy at someone, add them to the Include list.</span></span> <span data-ttu-id="5ce65-119">Per assicurarsi che una persona venga omessa dal criterio, aggiungerla all'elenco Escludi.</span><span class="sxs-lookup"><span data-stu-id="5ce65-119">To ensure that a person is omitted from the policy, add them to the Exclude list.</span></span>

<span data-ttu-id="5ce65-120">Collegamenti utili:</span><span class="sxs-lookup"><span data-stu-id="5ce65-120">Helpful links:</span></span>

[<span data-ttu-id="5ce65-121">Panoramica della conformità del dispositivo</span><span class="sxs-lookup"><span data-stu-id="5ce65-121">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="5ce65-122">Risoluzione dei problemi relativi all'autorità di certificazione</span><span class="sxs-lookup"><span data-stu-id="5ce65-122">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="5ce65-123">Risoluzione dei problemi relativi ai criteri</span><span class="sxs-lookup"><span data-stu-id="5ce65-123">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

[<span data-ttu-id="5ce65-124">Monitoraggio della conformità del dispositivo Intune</span><span class="sxs-lookup"><span data-stu-id="5ce65-124">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

<span data-ttu-id="5ce65-125">Nota: questi passaggi sono utili solo per la risoluzione dei problemi relativi all'accesso condizionale delle funzionalità di Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5ce65-125">Note: these steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="5ce65-126">È anche possibile mettere in quarantena un dispositivo che blocca l'accesso alla posta elettronica con i criteri di Exchange.</span><span class="sxs-lookup"><span data-stu-id="5ce65-126">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="5ce65-127">Ulteriori informazioni sulla gestione dei dispositivi di Exchange sono disponibili [qui](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).</span><span class="sxs-lookup"><span data-stu-id="5ce65-127">More information on Exchange device management can be found [here](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).</span></span>
