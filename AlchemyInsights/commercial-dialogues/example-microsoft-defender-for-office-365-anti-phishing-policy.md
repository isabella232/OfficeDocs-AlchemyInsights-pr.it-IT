---
title: Esempio di criterio anti-phishing di Microsoft Defender per Office 365
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: eabff70c22b641627d3ab6c0b2f8846a0be2f49e
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50737185"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a><span data-ttu-id="99022-102">Esempio di criterio anti-phishing di Microsoft Defender per Office 365</span><span class="sxs-lookup"><span data-stu-id="99022-102">Example Microsoft Defender for Office 365 anti-phishing policy</span></span>

<span data-ttu-id="99022-103">Queste impostazioni abilitano un criterio *denominato Dominio e CEO.*</span><span class="sxs-lookup"><span data-stu-id="99022-103">These settings enable a policy called *Domain and CEO*.</span></span> <span data-ttu-id="99022-104">Questo criterio fornisce protezione utente e dominio dalla rappresentazione e quindi applica il criterio a tutti i messaggi di posta elettronica ricevuti dagli utenti all'interno del dominio.</span><span class="sxs-lookup"><span data-stu-id="99022-104">This policy provides both user and domain protection from impersonation and then applies the policy to all email received by users within the domain.</span></span> <span data-ttu-id="99022-105">Innanzitutto, aggiungere le informazioni seguenti per creare il criterio:</span><span class="sxs-lookup"><span data-stu-id="99022-105">First, add the following information to create the policy:</span></span>

- <span data-ttu-id="99022-106">**Name**: Domain and CEO **Description**: Garantisce che il CEO e il dominio non vengano impersonati.</span><span class="sxs-lookup"><span data-stu-id="99022-106">**Name**: Domain and CEO **Description**: Ensures that the CEO and your domain are not being impersonated.</span></span>
  <span data-ttu-id="99022-107">**Applicato a**: selezionare **Il dominio del destinatario è**.</span><span class="sxs-lookup"><span data-stu-id="99022-107">**Applied to**: Select **The recipient domain is**.</span></span> <span data-ttu-id="99022-108">In **Uno di questi,** selezionare **Scegli** e quindi selezionare un dominio.</span><span class="sxs-lookup"><span data-stu-id="99022-108">Under **Any of these**, select **Choose**, and then select a domain.</span></span> <span data-ttu-id="99022-109">Selezionare **+ Aggiungi**.</span><span class="sxs-lookup"><span data-stu-id="99022-109">Select **+ Add**.</span></span> <span data-ttu-id="99022-110">Selezionare la casella di controllo accanto al nome del dominio nell'elenco , ad esempio *contoso.com*), quindi selezionare **Aggiungi**.</span><span class="sxs-lookup"><span data-stu-id="99022-110">Select the check box next to the name of the domain in the list (for example, *contoso.com*), and then select **Add**.</span></span> <span data-ttu-id="99022-111">Scegliere **Fatto**.</span><span class="sxs-lookup"><span data-stu-id="99022-111">Select **Done**.</span></span>
- <span data-ttu-id="99022-112">Dopo aver creato il criterio, è possibile ottimizzare il criterio utilizzando le opzioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="99022-112">After the policy is created, you can fine-tune the policy by using the following options:</span></span>
  - <span data-ttu-id="99022-113">**Aggiungere utenti da proteggere:** Per questo esempio, aggiungi almeno l'indirizzo di posta elettronica del CEO.</span><span class="sxs-lookup"><span data-stu-id="99022-113">**Add users to protect:** For this example, add the CEO's email address, at a minimum.</span></span>
  - <span data-ttu-id="99022-114">**Aggiungere domini da proteggere:** aggiungere il dominio dell'organizzazione che include l'ufficio del CEO.</span><span class="sxs-lookup"><span data-stu-id="99022-114">**Add domains to protect**: Add the organizational domain that includes the office of the CEO.</span></span>
  - <span data-ttu-id="99022-115">**Scegliere azioni**: **Per** Se la posta elettronica viene inviata da un utente *rappresentato,* selezionare Reindirizza il messaggio a un altro indirizzo **di** posta elettronica e quindi immettere l'indirizzo di posta elettronica dell'amministratore della sicurezza (ad esempio, securityadmin@contoso.com ).</span><span class="sxs-lookup"><span data-stu-id="99022-115">**Choose actions**: For **If email is sent by an impersonated user**, select **Redirect message to another email address**, and then enter the email address of the security administrator (for example, *securityadmin@contoso.com*).</span></span> <span data-ttu-id="99022-116">Per **Se la posta elettronica viene inviata da un dominio rappresentato,** selezionare **Metti in quarantena il messaggio.**</span><span class="sxs-lookup"><span data-stu-id="99022-116">For **If email is sent by an impersonated domain**, select **Quarantine the message**.</span></span>
  - <span data-ttu-id="99022-117">**Intelligence delle** cassette postali: per impostazione predefinita, questa opzione è selezionata quando si crea un nuovo criterio anti-phishing.</span><span class="sxs-lookup"><span data-stu-id="99022-117">**Mailbox intelligence**: By default, this option is selected when you create a new anti-phishing policy.</span></span> <span data-ttu-id="99022-118">Per ottenere risultati ottimali, lasciare l’opzione **attiva**.</span><span class="sxs-lookup"><span data-stu-id="99022-118">Leave this setting **On** for best results.</span></span>
  - <span data-ttu-id="99022-119">**Aggiungere mittenti e domini attendibili:** Per questo esempio, non definire sostituzioni.</span><span class="sxs-lookup"><span data-stu-id="99022-119">**Add trusted senders and domains:** For this example, don't define any overrides.</span></span>
- <span data-ttu-id="99022-120">Dopo aver esaminato le impostazioni, selezionare **Crea questo criterio** o **Salva**, come appropriato.</span><span class="sxs-lookup"><span data-stu-id="99022-120">Once you've reviewed your settings, select **Create this policy** or **Save**, as appropriate.</span></span>

<span data-ttu-id="99022-121">Per ulteriori informazioni, vedere [Criteri anti-phishing in Microsoft 365.](https://go.microsoft.com/fwlink/?linkid=2092235)</span><span class="sxs-lookup"><span data-stu-id="99022-121">To learn more, see [Anti-phishing policies in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).</span></span>
