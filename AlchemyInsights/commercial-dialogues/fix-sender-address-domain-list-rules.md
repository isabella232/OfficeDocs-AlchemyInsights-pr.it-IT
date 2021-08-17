---
title: Correggere indirizzo mittente/Regole elenco domini
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
ms.openlocfilehash: db8b921fc84f42b6cef1138dca9ad433e648e0a2f10e80927bd5b0222bfeae3b
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896115"
---
# <a name="fix-sender-addressdomain-list-rules"></a>Correggere indirizzo mittente/Regole elenco domini

Uno dei criteri di protezione da posta indesiderata ha interessato questo messaggio. Il mittente del messaggio è stato trovato in un elenco Consenti o Blocca. Per esaminare i criteri, eseguire la procedura seguente:

1. Nel portale Microsoft 365 Defender posta elettronica all'indirizzo , passare a Email <https://security.microsoft.com/> **& Collaboration** Policies & \> **Rules Threat** \> **policies** \> **Anti-spam** nella **sezione Criteri.**

   Per passare direttamente alla pagina **Criteri di protezione dalla posta indesiderata**, usare <https://security.microsoft.com/antispam>.

2. Nella pagina Criteri di protezione da posta indesiderata selezionare il criterio facendo clic sul nome del criterio **(** Type is Custom **anti-spam** **policy** o **Name** is **Anti-Spam inbound policy (Default)**.
3. Nel riquadro a comparsa dei dettagli visualizzato selezionare **Modifica** mittenti e domini consentiti e bloccati nella sezione **Mittenti e** domini consentiti e bloccati.
4. Nella sezione **Consentito** esaminare i mittenti e i domini facendo clic **su Gestisci \<nn\> mittenti** o **Consenti domini**.

Per altre informazioni, vedere [Configurare i criteri di protezione dalla posta indesiderata in EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-your-spam-filter-policies).
