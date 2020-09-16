---
title: Le etichette di riservatezza non vengono visualizzate
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 6a64e001be115c8e5553a0d8c97b8cb815922c69
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801188"
---
# <a name="sensitivity-labels-not-appearing"></a><span data-ttu-id="6faac-102">Le etichette di riservatezza non vengono visualizzate</span><span class="sxs-lookup"><span data-stu-id="6faac-102">Sensitivity labels not appearing</span></span>

<span data-ttu-id="6faac-103">Le etichette di riservatezza consentono di classificare e proteggere i contenuti sensibili.</span><span class="sxs-lookup"><span data-stu-id="6faac-103">Sensitivity labels allow you to classify and help protect your sensitive content.</span></span> <span data-ttu-id="6faac-104">Possono essere creati in Microsoft 365 Compliance Center, Microsoft 365 Security Center o Microsoft 365 Security & Compliance Center in Classification > Sensitivity labels.</span><span class="sxs-lookup"><span data-stu-id="6faac-104">They can be created in the Microsoft 365 compliance center, Microsoft 365 security center, or Microsoft 365 security & Compliance Center under Classification > Sensitivity labels.</span></span> <span data-ttu-id="6faac-105">Per ulteriori informazioni su questa funzionalità, vedere [Overview of Sensitivity labels](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).</span><span class="sxs-lookup"><span data-stu-id="6faac-105">To learn more about this feature, see [Overview of sensitivity labels](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).</span></span>

<span data-ttu-id="6faac-106">Se le etichette di riservatezza sono state configurate ma non vengono visualizzate nelle app Microsoft 365, controllare quanto segue:</span><span class="sxs-lookup"><span data-stu-id="6faac-106">If you configured your sensitivity labels but they aren't appearing in the Microsoft 365 apps, check the following:</span></span>

- <span data-ttu-id="6faac-107">Verificare che l'etichetta di riservatezza sia stata [pubblicata](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) per gli utenti e i gruppi desiderati.</span><span class="sxs-lookup"><span data-stu-id="6faac-107">Confirm that the sensitivity label has been [published](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) to the users and groups that you want.</span></span>

- <span data-ttu-id="6faac-108">Verificare che l'utente stia utilizzando un'app che supporta le etichette di riservatezza: vedere [etichette di riservatezza nel documento](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).</span><span class="sxs-lookup"><span data-stu-id="6faac-108">Confirm that the user is using an app that supports sensitivity labels - see [sensitivity labels in your document](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).</span></span>

- <span data-ttu-id="6faac-109">Se si sta [eseguendo la migrazione delle etichette di Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), tenere conto delle considerazioni riportate di [seguito](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).</span><span class="sxs-lookup"><span data-stu-id="6faac-109">If you're [migrating Azure Information Protection labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), be aware of the considerations listed [here](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).</span></span>

- <span data-ttu-id="6faac-110">Supporto per la prevenzione della perdita di dati (DLP): attualmente, solo le etichette di conservazione possono essere utilizzate come condizione nei criteri DLP.</span><span class="sxs-lookup"><span data-stu-id="6faac-110">Data loss prevention (DLP) support: Currently, only retention labels can be used as a condition in DLP policies.</span></span>  <span data-ttu-id="6faac-111">Il supporto per le etichette di riservatezza in un criterio DLP non è ancora disponibile, ma ci stiamo lavorando.</span><span class="sxs-lookup"><span data-stu-id="6faac-111">Support for sensitivity labels in a DLP policy is not available yet but we're working on it.</span></span>

- <span data-ttu-id="6faac-112">Quando la crittografia è abilitata su un'etichetta di riservatezza, è possibile scegliere di:</span><span class="sxs-lookup"><span data-stu-id="6faac-112">When encryption is enabled on a sensitivity label, you can choose either to:</span></span>
    - <span data-ttu-id="6faac-113">Assegnare le autorizzazioni adesso</span><span class="sxs-lookup"><span data-stu-id="6faac-113">Assign permissions now</span></span>
    - <span data-ttu-id="6faac-114">Consentire agli utenti di assegnare le autorizzazioni</span><span class="sxs-lookup"><span data-stu-id="6faac-114">Let users assign permissions</span></span>


<span data-ttu-id="6faac-115">Per ulteriori informazioni sui possibili problemi, vedere [problemi noti relativi alle etichette di riservatezza](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span><span class="sxs-lookup"><span data-stu-id="6faac-115">For more information on possible issues, see [Known issues with sensitivity labels](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span></span>