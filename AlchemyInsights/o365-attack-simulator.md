---
title: 2681 Attack Simulator in Microsoft 365
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
- "2681"
ms.assetid: ''
ms.openlocfilehash: e7d71fdb77b4a047c1998e9aba75cdd469a936a8
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545730"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="031da-102">Simulatore di attacco in Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="031da-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="031da-103">Simulatore di attacco mancante?</span><span class="sxs-lookup"><span data-stu-id="031da-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="031da-104">Attack Simulator richiede **Microsoft Defender per Office 365 Piano 2** o Office 365 Enterprise **E5.**</span><span class="sxs-lookup"><span data-stu-id="031da-104">Attack Simulator requires **Microsoft Defender for Office 365 Plan 2** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="031da-105">Il simulatore **di attacco** non è incluso in Microsoft Defender per Office 365 Piano 1, Office 365 Enterprise E3 o in Microsoft 365 Apps for business abbonamenti.</span><span class="sxs-lookup"><span data-stu-id="031da-105">Attack Simulator is **not** included in Microsoft Defender for Office 365 Plan 1, Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="031da-106">L'account utilizzato per avviare attacchi simulati richiede autorizzazioni di amministratore globale o amministratore della sicurezza e autenticazione a più fattori (MFA).</span><span class="sxs-lookup"><span data-stu-id="031da-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="031da-107">Per ulteriori informazioni sui requisiti del simulatore di attacco, vedere [questo argomento.](/microsoft-365/security/office-365-security/attack-simulator)</span><span class="sxs-lookup"><span data-stu-id="031da-107">For more information about Attack Simulator requirements, see [this topic](/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="031da-108">Aspetti importanti da sapere sulle simulazioni di attacco **Brute Force Password:**</span><span class="sxs-lookup"><span data-stu-id="031da-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="031da-109">Se l'account di destinazione ha la MFA abilitata e la password è stata indovinata correttamente, l'account non verrà visualizzato come compromesso (il secondo fattore di autenticazione sarà incompleto).</span><span class="sxs-lookup"><span data-stu-id="031da-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="031da-110">Il file delle password non può essere superiore a 10 MB.</span><span class="sxs-lookup"><span data-stu-id="031da-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="031da-111">Utilizzare una password per riga e includere una riga vuota (ritorno a capo) dopo l'ultima password nell'elenco.</span><span class="sxs-lookup"><span data-stu-id="031da-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="031da-112">Aspetti importanti da sapere sulle **simulazioni di attacco spear phishing:**</span><span class="sxs-lookup"><span data-stu-id="031da-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="031da-113">Per impostazione predefinita, non è possibile fornire un valore personalizzato per l'URL del **server di accesso phishing.**</span><span class="sxs-lookup"><span data-stu-id="031da-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="031da-114">Se un destinatario utilizza il componente aggiuntivo Segnala messaggio per segnalare il messaggio come phishing, è possibile che non si ricevano avvisi per il messaggio (perché si tratta di un attacco simulato). [](/microsoft-365/security/office-365-security/enable-the-report-message-add-in)</span><span class="sxs-lookup"><span data-stu-id="031da-114">If a recipient uses the [Enable the Report Message add-in](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="031da-115">Report: al termine dell'attacco simulato, è possibile fare clic su **Dettagli attacco** per visualizzare il report.</span><span class="sxs-lookup"><span data-stu-id="031da-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="031da-116">Per istruzioni dettagliate e nuove funzionalità in Attack Simulator, vedi [Simulatore](/microsoft-365/security/office-365-security/attack-simulator)di attacco in Microsoft 365 .</span><span class="sxs-lookup"><span data-stu-id="031da-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](/microsoft-365/security/office-365-security/attack-simulator).</span></span>
