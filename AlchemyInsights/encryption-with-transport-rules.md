---
title: Crittografia con le regole di trasporto
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5154"
ms.openlocfilehash: 4c43fc16db84832c4e2aa3b6483632de6861b877
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47784347"
---
# <a name="encryption-with-transport-rules"></a><span data-ttu-id="a51d4-102">Crittografia con le regole di trasporto</span><span class="sxs-lookup"><span data-stu-id="a51d4-102">Encryption with transport rules</span></span>

<span data-ttu-id="a51d4-103">Nell'[interfaccia di amministrazione di Exchange](https://go.microsoft.com/fwlink/p/?linkid=834822) è possibile usare le funzionalità di Crittografia messaggi di Office nelle regole del flusso di posta per attivare la crittografia dei messaggi.</span><span class="sxs-lookup"><span data-stu-id="a51d4-103">In the [Exchange Admin Center](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC), you can use Office Message Encryption(OME) capabilities in your mail flow rules to trigger message encryption.</span></span> <span data-ttu-id="a51d4-104">Scegliere l'opzione **Applica Office 365 Message Encryption e la protezione tramite diritti** nella condizione della regola di trasporto.</span><span class="sxs-lookup"><span data-stu-id="a51d4-104">Choose the **Apply Office 365 Message Encryption and rights protection** option on the Transport Rule condition.</span></span>

- <span data-ttu-id="a51d4-105">Per ulteriori informazioni, vedere [Definire la regola del flusso di posta per la crittografia](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span><span class="sxs-lookup"><span data-stu-id="a51d4-105">For more information, see [Define Mail flow rule to encrypt](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span></span>

- <span data-ttu-id="a51d4-106">In PowerShell usare il cmdlet [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) e impostare il parametro *ApplyOME* su $true.</span><span class="sxs-lookup"><span data-stu-id="a51d4-106">In Powershell, use the [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) cmdlet and set the *ApplyOME* parameter to $true.</span></span>
