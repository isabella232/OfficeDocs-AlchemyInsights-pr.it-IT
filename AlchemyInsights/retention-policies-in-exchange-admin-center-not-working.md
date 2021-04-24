---
title: Criteri di conservazione nell'interfaccia di amministrazione di Exchange non funzionanti
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: bb2ce7ce2405be575dfdb79d304fef690e863a4e
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952232"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="9a0ff-102">Criteri di conservazione nell'interfaccia di amministrazione di Exchange</span><span class="sxs-lookup"><span data-stu-id="9a0ff-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="9a0ff-103">Se si desidera eseguire controlli automatizzati per le impostazioni indicate di seguito, selezionare il pulsante Indietro <, nella parte superiore di questa pagina, quindi immettere l'indirizzo di posta elettronica dell'utente che ha problemi con i criteri di conservazione.</span><span class="sxs-lookup"><span data-stu-id="9a0ff-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

<span data-ttu-id="9a0ff-104">Se si verificano problemi con i criteri di conservazione nell'interfaccia di amministrazione di Exchange che non si applicano alle cassette postali o agli elementi che non si spostano nella cassetta postale di archiviazione, controllare quanto segue:</span><span class="sxs-lookup"><span data-stu-id="9a0ff-104">If you have problems with retention policies in the Exchange Admin Center not applying to mailboxes or items not moving to the archive mailbox, check the following:</span></span>

<span data-ttu-id="9a0ff-105">**Cause radice:**</span><span class="sxs-lookup"><span data-stu-id="9a0ff-105">**Root Causes:**</span></span>

- <span data-ttu-id="9a0ff-106">**L'Assistente cartelle** gestite non ha elaborato la cassetta postale dell'utente.</span><span class="sxs-lookup"><span data-stu-id="9a0ff-106">**Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="9a0ff-107">L'Assistente cartelle gestite tenta di elaborare ogni cassetta postale nell'organizzazione basata su cloud una volta ogni sette giorni.</span><span class="sxs-lookup"><span data-stu-id="9a0ff-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span>

  <span data-ttu-id="9a0ff-108">**Soluzione:** Eseguire l'Assistente cartelle gestite.</span><span class="sxs-lookup"><span data-stu-id="9a0ff-108">**Solution:** Run the Managed Folder Assistant.</span></span>

- <span data-ttu-id="9a0ff-109">**RetentionHold** è stato **abilitato** nella cassetta postale.</span><span class="sxs-lookup"><span data-stu-id="9a0ff-109">**RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="9a0ff-110">Se la cassetta postale è stata impostata su RetentionHold, il criterio di conservazione sulla cassetta postale non verrà elaborato durante tale periodo.</span><span class="sxs-lookup"><span data-stu-id="9a0ff-110">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span>

  <span data-ttu-id="9a0ff-111">**Soluzione:** Controllare lo stato dell'impostazione del blocco di conservazione e aggiornare in base alle esigenze.</span><span class="sxs-lookup"><span data-stu-id="9a0ff-111">**Solution:** Check status of Retention Hold setting and update as needed.</span></span> <span data-ttu-id="9a0ff-112">Per informazioni dettagliate, vedere [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="9a0ff-112">For details, see [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
 
<span data-ttu-id="9a0ff-113">**Nota:** Se una cassetta postale è inferiore a 10 MB, l'Assistente cartelle gestite non eelaborare automaticamente la cassetta postale.</span><span class="sxs-lookup"><span data-stu-id="9a0ff-113">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="9a0ff-114">Per altre info sui criteri di conservazione nell'interfaccia di amministrazione di Exchange, vedi:</span><span class="sxs-lookup"><span data-stu-id="9a0ff-114">For more info on retention policies in the Exchange Admin Center, see:</span></span>

- [<span data-ttu-id="9a0ff-115">Tag di conservazione e criteri di conservazione</span><span class="sxs-lookup"><span data-stu-id="9a0ff-115">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- <span data-ttu-id="9a0ff-116">[Applicare un criterio di conservazione alle cassette postali](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) o Aggiungere o rimuovere tag di [conservazione](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span><span class="sxs-lookup"><span data-stu-id="9a0ff-116">[Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) or [Add or remove retention tags](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span></span>

- [<span data-ttu-id="9a0ff-117">Come identificare il tipo di blocco applicato a una cassetta postale</span><span class="sxs-lookup"><span data-stu-id="9a0ff-117">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
