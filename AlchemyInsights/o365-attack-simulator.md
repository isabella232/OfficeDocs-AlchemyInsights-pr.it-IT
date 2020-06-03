---
title: 2681 Attack Simulator in Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 3dae4768ca62757ce7f92dfc527078c963d72742
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506742"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="da69f-102">Simulatore di attacco in Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="da69f-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="da69f-103">Si sta perdendo il simulatore d'attacco?</span><span class="sxs-lookup"><span data-stu-id="da69f-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="da69f-104">Attack Simulator richiede **office 365 Advanced Threat Protection Plan 2 (ATP piano 2)** o **Office 365 Enterprise E5**.</span><span class="sxs-lookup"><span data-stu-id="da69f-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="da69f-105">Attacco Simulator **non** è incluso in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3 o qualsiasi Microsoft 365 Apps for business abbonamenti.</span><span class="sxs-lookup"><span data-stu-id="da69f-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="da69f-106">L'account utilizzato per avviare gli attacchi simulati richiede l'amministratore globale o le autorizzazioni di amministratore della sicurezza e l'autenticazione a più fattori (AMF).</span><span class="sxs-lookup"><span data-stu-id="da69f-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="da69f-107">Per ulteriori informazioni sui requisiti dei simulatori di attacco, vedere [questo argomento](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="da69f-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="da69f-108">Aspetti importanti da sapere sulle simulazioni di attacchi di password per la **forza bruta** :</span><span class="sxs-lookup"><span data-stu-id="da69f-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="da69f-109">Se l'account di destinazione è abilitato per l'utilizzo dell'AMF e la password è stata indovinata, l'account non verrà visualizzato come compromesso (il secondo fattore di autenticazione sarà incompleto).</span><span class="sxs-lookup"><span data-stu-id="da69f-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="da69f-110">Il file della password non può essere superiore a 10 MB.</span><span class="sxs-lookup"><span data-stu-id="da69f-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="da69f-111">Utilizzare una password per riga e includere una riga vuota (ritorno a capo) dopo l'ultima password dell'elenco.</span><span class="sxs-lookup"><span data-stu-id="da69f-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="da69f-112">Aspetti importanti da sapere sulle simulazioni di attacchi di **phishing Spear** :</span><span class="sxs-lookup"><span data-stu-id="da69f-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="da69f-113">In base alla progettazione, non è possibile specificare un valore personalizzato per l' **URL del server di accesso di phishing**.</span><span class="sxs-lookup"><span data-stu-id="da69f-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="da69f-114">Se un destinatario utilizza il [componente aggiuntivo attiva messaggio di report](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) per segnalare il messaggio come phishing, potrebbe non essere possibile ricevere avvisi per il messaggio (poiché si tratta di un attacco simulato).</span><span class="sxs-lookup"><span data-stu-id="da69f-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="da69f-115">Report: dopo aver completato l'attacco simulato, è possibile fare clic su **Dettagli attacco** per visualizzare il report.</span><span class="sxs-lookup"><span data-stu-id="da69f-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="da69f-116">Per istruzioni dettagliate e nuove funzionalità in Attack Simulator, vedere [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="da69f-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
