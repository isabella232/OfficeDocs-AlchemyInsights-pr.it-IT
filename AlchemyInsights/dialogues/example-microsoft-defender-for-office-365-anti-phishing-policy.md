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
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/08/2021
ms.locfileid: "50552421"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a><span data-ttu-id="c5363-102">Esempio di criterio anti-phishing di Microsoft Defender per Office 365</span><span class="sxs-lookup"><span data-stu-id="c5363-102">Example Microsoft Defender for Office 365 anti-phishing policy</span></span>

<span data-ttu-id="c5363-103">Queste impostazioni abilitano un criterio *denominato Dominio e CEO.*</span><span class="sxs-lookup"><span data-stu-id="c5363-103">These settings enable a policy called *Domain and CEO*.</span></span> <span data-ttu-id="c5363-104">Questo criterio fornisce la protezione sia dell'utente che del dominio dalla rappresentazione e quindi applica il criterio a tutti i messaggi di posta elettronica ricevuti dagli utenti all'interno del dominio.</span><span class="sxs-lookup"><span data-stu-id="c5363-104">This policy provides both user and domain protection from impersonation and then applies the policy to all email received by users within the domain.</span></span> <span data-ttu-id="c5363-105">Innanzitutto, aggiungere le informazioni seguenti per creare il criterio:</span><span class="sxs-lookup"><span data-stu-id="c5363-105">First, add the following information to create the policy:</span></span>

- <span data-ttu-id="c5363-106">**Name**: Domain and CEO **Description**: Ensures that the CEO and your domain are not being impersonated.</span><span class="sxs-lookup"><span data-stu-id="c5363-106">**Name**: Domain and CEO **Description**: Ensures that the CEO and your domain are not being impersonated.</span></span>
  <span data-ttu-id="c5363-107">**Applicato a**: Selezionare **il dominio del destinatario.**</span><span class="sxs-lookup"><span data-stu-id="c5363-107">**Applied to**: Select **The recipient domain is**.</span></span> <span data-ttu-id="c5363-108">In **Una di queste opzioni** selezionare **Scegli** e quindi selezionare un dominio.</span><span class="sxs-lookup"><span data-stu-id="c5363-108">Under **Any of these**, select **Choose**, and then select a domain.</span></span> <span data-ttu-id="c5363-109">Selezionare **+ Aggiungi**.</span><span class="sxs-lookup"><span data-stu-id="c5363-109">Select **+ Add**.</span></span> <span data-ttu-id="c5363-110">Selezionare la casella di controllo accanto al nome del dominio nell'elenco , ad esempio *contoso.com*), quindi selezionare **Aggiungi**.</span><span class="sxs-lookup"><span data-stu-id="c5363-110">Select the check box next to the name of the domain in the list (for example, *contoso.com*), and then select **Add**.</span></span> <span data-ttu-id="c5363-111">Scegliere **Fatto**.</span><span class="sxs-lookup"><span data-stu-id="c5363-111">Select **Done**.</span></span>
- <span data-ttu-id="c5363-112">Dopo aver creato il criterio, è possibile ottimizzare il criterio utilizzando le opzioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="c5363-112">After the policy is created, you can fine-tune the policy by using the following options:</span></span>
  - <span data-ttu-id="c5363-113">**Aggiungere utenti da proteggere:** Per questo esempio, aggiungere almeno l'indirizzo di posta elettronica del CEO.</span><span class="sxs-lookup"><span data-stu-id="c5363-113">**Add users to protect:** For this example, add the CEO's email address, at a minimum.</span></span>
  - <span data-ttu-id="c5363-114">**Aggiungere domini da proteggere:** aggiungere il dominio dell'organizzazione che include l'ufficio del CEO.</span><span class="sxs-lookup"><span data-stu-id="c5363-114">**Add domains to protect**: Add the organizational domain that includes the office of the CEO.</span></span>
  - <span data-ttu-id="c5363-115">**Choose actions**: For **If email is sent by an impersonated user,** select **Redirect message to another email address**, and then enter the email address of the security administrator (for example, *securityadmin@contoso.com*).</span><span class="sxs-lookup"><span data-stu-id="c5363-115">**Choose actions**: For **If email is sent by an impersonated user**, select **Redirect message to another email address**, and then enter the email address of the security administrator (for example, *securityadmin@contoso.com*).</span></span> <span data-ttu-id="c5363-116">Per **Se la posta elettronica viene inviata da un dominio rappresentato,** selezionare **Metti in quarantena il messaggio.**</span><span class="sxs-lookup"><span data-stu-id="c5363-116">For **If email is sent by an impersonated domain**, select **Quarantine the message**.</span></span>
  - <span data-ttu-id="c5363-117">**Intelligence per le** cassette postali: per impostazione predefinita, questa opzione è selezionata quando si crea un nuovo criterio anti-phishing.</span><span class="sxs-lookup"><span data-stu-id="c5363-117">**Mailbox intelligence**: By default, this option is selected when you create a new anti-phishing policy.</span></span> <span data-ttu-id="c5363-118">Per ottenere risultati ottimali, lasciare l’opzione **attiva**.</span><span class="sxs-lookup"><span data-stu-id="c5363-118">Leave this setting **On** for best results.</span></span>
  - <span data-ttu-id="c5363-119">**Aggiungere domini e mittenti attendibili:** Per questo esempio, non definire sostituzioni.</span><span class="sxs-lookup"><span data-stu-id="c5363-119">**Add trusted senders and domains:** For this example, don't define any overrides.</span></span>
- <span data-ttu-id="c5363-120">Dopo aver esaminato le impostazioni, selezionare Crea **questo criterio** o **Salva**, in base alle esigenze.</span><span class="sxs-lookup"><span data-stu-id="c5363-120">Once you've reviewed your settings, select **Create this policy** or **Save**, as appropriate.</span></span>

<span data-ttu-id="c5363-121">Per ulteriori informazioni, vedere [Criteri anti-phishing in Microsoft 365.](https://go.microsoft.com/fwlink/?linkid=2092235)</span><span class="sxs-lookup"><span data-stu-id="c5363-121">To learn more, see [Anti-phishing policies in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).</span></span>
