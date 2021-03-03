---
title: Monitorare l'accesso condizionale di Intune
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/03/2021
ms.locfileid: "50417317"
---
# <a name="monitor-intune-conditional-access"></a><span data-ttu-id="969f4-102">Monitorare l'accesso condizionale di Intune</span><span class="sxs-lookup"><span data-stu-id="969f4-102">Monitor Intune Conditional Access</span></span>

<span data-ttu-id="969f4-103">Gli utenti con accesso condizionale riceveranno un messaggio di posta elettronica di notifica se non soddisfano i requisiti di accesso dell'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="969f4-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="969f4-104">Per risolvere il problema, è consigliabile utilizzare una o più delle soluzioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="969f4-104">To resolve, we recommend one or more of the following solutions:</span></span>

1. <span data-ttu-id="969f4-105">Se si presume che il dispositivo sia registrato, consigliare all'utente di passare all'app Portale aziendale e verificare che venga visualizzato nel portale aziendale.</span><span class="sxs-lookup"><span data-stu-id="969f4-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="969f4-106">In caso contrario, l'utente deve registrare il dispositivo.</span><span class="sxs-lookup"><span data-stu-id="969f4-106">If it doesn't, the user must enroll the device.</span></span>
1. <span data-ttu-id="969f4-107">Nel portale di Azure passare a **Conformità dei dispositivi**  >  **di** Intune.</span><span class="sxs-lookup"><span data-stu-id="969f4-107">In the Azure portal go to **Intune** > **Device compliance**.</span></span> 
1. <span data-ttu-id="969f4-108">Per visualizzare il report di conformità del dispositivo per verificare che il dispositivo dell'utente sia contrassegnato come conforme, in **Monitoraggio** fare clic su **Conformità dispositivo.**</span><span class="sxs-lookup"><span data-stu-id="969f4-108">To view your device compliance report to verify that the user's device is marked as compliant, under **Monitor**, click **Device compliance**.</span></span>
1. <span data-ttu-id="969f4-109">Nel portale di Azure passare a **Conformità dei dispositivi**  >  **di** Intune.</span><span class="sxs-lookup"><span data-stu-id="969f4-109">In the Azure portal go to **Intune** > **Device compliance**.</span></span> <span data-ttu-id="969f4-110">In **Gestisci fare clic** su **Criteri.**</span><span class="sxs-lookup"><span data-stu-id="969f4-110">Under **Manage,** click **Policies**.</span></span> <span data-ttu-id="969f4-111">Nell'elenco dei criteri di conformità, verificare che un profilo sia assegnato al dispositivo dell'utente.</span><span class="sxs-lookup"><span data-stu-id="969f4-111">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="969f4-112">Se non è assegnato alcun profilo, Intune non sarà in grado di confermare lo stato di conformità del dispositivo.</span><span class="sxs-lookup"><span data-stu-id="969f4-112">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
1. <span data-ttu-id="969f4-113">Modificare l'assegnazione di accesso condizionale dell'utente.</span><span class="sxs-lookup"><span data-stu-id="969f4-113">Edit the user's conditional access assignment.</span></span>
1. <span data-ttu-id="969f4-114">Nel portale di Azure passare a Criteri di accesso condizionale di **Intune,** selezionare un criterio dall'elenco e fare clic  >    >  su Utenti **e gruppi.**</span><span class="sxs-lookup"><span data-stu-id="969f4-114">In the Azure portal, navigate to **Intune** > **Conditional access** > **Policies**, select a policy from the list, and click **Users and groups**.</span></span>
1. <span data-ttu-id="969f4-115">Per impostare un determinato criterio come destinatario, aggiungerlo **all'elenco Includi.**</span><span class="sxs-lookup"><span data-stu-id="969f4-115">To target a certain policy at someone, add them to the **Include list**.</span></span> <span data-ttu-id="969f4-116">Per assicurarsi che una persona sia omessa dal criterio, aggiungerla **all'elenco Escludi.**</span><span class="sxs-lookup"><span data-stu-id="969f4-116">To ensure that a person is omitted from the policy, add them to the **Exclude list**.</span></span>

<span data-ttu-id="969f4-117">**Collegamenti utili:**</span><span class="sxs-lookup"><span data-stu-id="969f4-117">**Helpful links:**</span></span>

- [<span data-ttu-id="969f4-118">Panoramica della conformità dei dispositivi</span><span class="sxs-lookup"><span data-stu-id="969f4-118">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)
- [<span data-ttu-id="969f4-119">Risoluzione dei problemi dell'autorità di certificazione</span><span class="sxs-lookup"><span data-stu-id="969f4-119">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [<span data-ttu-id="969f4-120">Criteri per la risoluzione dei problemi</span><span class="sxs-lookup"><span data-stu-id="969f4-120">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [<span data-ttu-id="969f4-121">Monitoraggio della conformità dei dispositivi Intune</span><span class="sxs-lookup"><span data-stu-id="969f4-121">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> <span data-ttu-id="969f4-122">Questi passaggi sono utili solo per la risoluzione dei problemi relativi alla funzionalità accesso condizionale di Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="969f4-122">These steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="969f4-123">È anche possibile mettere in quarantena un dispositivo che blocca l'accesso alla posta elettronica con i criteri di Exchange.</span><span class="sxs-lookup"><span data-stu-id="969f4-123">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="969f4-124">Ulteriori informazioni sulla gestione dei dispositivi di Exchange sono disponibili [**qui.**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141))</span><span class="sxs-lookup"><span data-stu-id="969f4-124">More information on Exchange device management can be found [**here**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).</span></span>
