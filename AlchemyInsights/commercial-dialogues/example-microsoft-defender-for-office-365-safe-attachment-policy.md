---
title: Esempio di criterio allegati sicuri di Microsoft Defender per Office 365
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
ms.openlocfilehash: 077762dd37a2974b4e519c1f242fa753623cb49a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736750"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a><span data-ttu-id="139a7-102">Esempio di criterio allegati sicuri di Microsoft Defender per Office 365</span><span class="sxs-lookup"><span data-stu-id="139a7-102">Example Microsoft Defender for Office 365 Safe Attachment policy</span></span>

<span data-ttu-id="139a7-103">Queste impostazioni abilitano un criterio denominato *Nessun* ritardo che recapita immediatamente i messaggi e quindi ricollegare gli allegati dopo l'analisi:</span><span class="sxs-lookup"><span data-stu-id="139a7-103">These settings enable a policy called *No delays* that delivers messages immediately and then reattaches attachments after they're scanned:</span></span>

- <span data-ttu-id="139a7-104">**Nome**: Nessun ritardo</span><span class="sxs-lookup"><span data-stu-id="139a7-104">**Name**: No delays</span></span>
- <span data-ttu-id="139a7-105">**Descrizione:** recapita immediatamente i messaggi e ricollegare gli allegati dopo l'analisi.</span><span class="sxs-lookup"><span data-stu-id="139a7-105">**Description**: Delivers messages immediately and reattaches attachments after scanning.</span></span>
- <span data-ttu-id="139a7-106">**Risposta:** selezionare **l'opzione Recapito** dinamico.</span><span class="sxs-lookup"><span data-stu-id="139a7-106">**Response**: Select the **Dynamic Delivery** option.</span></span> <span data-ttu-id="139a7-107">Per ulteriori informazioni, vedere [Recapito dinamico nei criteri allegati sicuri.](https://go.microsoft.com/fwlink/?linkid=2092328)</span><span class="sxs-lookup"><span data-stu-id="139a7-107">For more information, see [Dynamic Delivery in Safe Attachments policies](https://go.microsoft.com/fwlink/?linkid=2092328).</span></span>
- <span data-ttu-id="139a7-108">**Sezione** Reindirizza allegato: selezionare l'opzione Abilita reindirizzamento **e** quindi immettere l'indirizzo di posta elettronica dell'amministratore globale di Microsoft 365, dell'amministratore della sicurezza o dell'analista della sicurezza che analista della sicurezza analgherà gli allegati dannosi.</span><span class="sxs-lookup"><span data-stu-id="139a7-108">**Redirect attachment** section: Select the option to **Enable redirect**, and then enter the email address of your Microsoft 365 global administrator, security administrator, or security analyst who will investigate malicious attachments.</span></span>
- <span data-ttu-id="139a7-109">**Sezione Applicato a:** selezionare **Il dominio del destinatario è** e quindi selezionare il dominio.</span><span class="sxs-lookup"><span data-stu-id="139a7-109">**Applied To** section: Select **The recipient domain is**, and then select your domain.</span></span> <span data-ttu-id="139a7-110">Selezionare **aggiungi** e quindi fare clic su **OK.**</span><span class="sxs-lookup"><span data-stu-id="139a7-110">Select **add**, and then select **OK**.</span></span> <span data-ttu-id="139a7-111">Al termine, selezionare **Salva**.</span><span class="sxs-lookup"><span data-stu-id="139a7-111">Once you're finished, select **Save**.</span></span>

<span data-ttu-id="139a7-112">Per ulteriori informazioni, vedere [Allegati sicuri in Microsoft Defender per Office 365.](https://go.microsoft.com/fwlink/?linkid=2092213)</span><span class="sxs-lookup"><span data-stu-id="139a7-112">To learn more, see [Safe Attachments in Microsoft Defender for Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).</span></span>
