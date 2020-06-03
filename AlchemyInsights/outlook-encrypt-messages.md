---
title: S/MIME in Outlook sul Web
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 6bbbf8722dacb8b7d5191d57ce1055a48dcb4dd0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511512"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="35cdf-102">Crittografare i messaggi di posta elettronica in Outlook</span><span class="sxs-lookup"><span data-stu-id="35cdf-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="35cdf-103">La crittografia dei messaggi di Microsoft 365 è basata su Microsoft Azure Rights Management (Azure RMS), che fa parte di Azure Information Protection.</span><span class="sxs-lookup"><span data-stu-id="35cdf-103">Microsoft 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="35cdf-104">Se l'abbonamento include Azure Rights Management o Azure Information Protection, **non è necessario eseguire alcuna azione per attivare o disattivare manualmente** il servizio Rights Management.</span><span class="sxs-lookup"><span data-stu-id="35cdf-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="35cdf-105">In base al feedback dei clienti, non è più possibile abilitare le regole del flusso di posta di Exchange per crittografare automaticamente la posta elettronica in uscita contenente alcuni tipi di informazioni riservate nel tenant per impostazione predefinita.</span><span class="sxs-lookup"><span data-stu-id="35cdf-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="35cdf-106">Al contrario, vengono fornite istruzioni dettagliate su come è possibile farlo da soli.</span><span class="sxs-lookup"><span data-stu-id="35cdf-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="35cdf-107">Per ulteriori informazioni su come creare una regola di trasporto per crittografare le informazioni riservate, vedere [questo articolo](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="35cdf-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="35cdf-108">Se si utilizza Outlook sul Web (in precedenza **OWA**): quando si compone un messaggio di posta elettronica, è sufficiente fare clic su **Proteggi** in OWA.</span><span class="sxs-lookup"><span data-stu-id="35cdf-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="35cdf-109">Verrà applicata l'autorizzazione "non inoltrare".</span><span class="sxs-lookup"><span data-stu-id="35cdf-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="35cdf-110">Fare clic su **Cambia autorizzazione** e scegliere **Crittografa** solo per crittografare il messaggio.</span><span class="sxs-lookup"><span data-stu-id="35cdf-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="35cdf-111">Se si utilizza il **client di Outlook**: per inviare un messaggio crittografato da Outlook 2013 o 2016 o Outlook 2016 per Mac, selezionare **Opzioni**  >  **autorizzazioni**, quindi selezionare l'opzione di protezione necessaria.</span><span class="sxs-lookup"><span data-stu-id="35cdf-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="35cdf-112">Per **crittografare automaticamente tutti i messaggi di posta elettronica** inviati a determinati destinatari o organizzazioni partner esterne, è necessario creare una regola di trasporto del flusso di posta nell'interfaccia di amministrazione di Exchange.</span><span class="sxs-lookup"><span data-stu-id="35cdf-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="35cdf-113">Istruzioni dettagliate sono disponibili in [questo articolo del supporto tecnico](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="35cdf-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

