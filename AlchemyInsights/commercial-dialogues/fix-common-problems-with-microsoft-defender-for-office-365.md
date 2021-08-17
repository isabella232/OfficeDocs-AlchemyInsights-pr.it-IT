---
title: Risolvere i problemi comuni con Microsoft Defender per Office 365
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
ms.openlocfilehash: 9104615baa5bf6dc91468912168e42ece6727eadd5330f1eb34e2a9170568b26
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/11/2021
ms.locfileid: "57898248"
---
# <a name="fix-common-problems-with-microsoft-defender-for-office-365"></a>Risolvere i problemi comuni con Microsoft Defender per Office 365

Ecco alcune soluzioni ai problemi comuni relativi a Microsoft Defender per Office 365:

- **Ritardo messaggio**:

  I ritardi nel recapito della posta elettronica potrebbero essere causati dall Cassaforte asalvamento dei messaggi da parte degli allegati. Per ulteriori informazioni, vedere impostazioni [Cassaforte dei criteri allegati](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-attachments#safe-attachments-policy-settings).

- **Segnalare risultati falsi positivi o negativi**:

  Per altre informazioni, vedere [Segnalazione di messaggi e file a Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-messages-to-microsoft).

- **Abilita Cassaforte protezione dei collegamenti:**

  1. Nel portale di Microsoft 365 Defender all'indirizzo , passare a Criteri di collaborazione & di posta elettronica & regole Criteri di Cassaforte <https://security.microsoft.com/>  \>  \>  \> **collegamenti nella** **sezione** Criteri.

     Per passare direttamente alla pagina **Cassaforte collegamenti,** utilizzare <https://security.microsoft.com/safelinksv2> .

  2. Nella pagina **Cassaforte collegamenti** selezionare il criterio facendo clic sul nome del criterio.
  3. Nel riquadro a comparsa dei dettagli visualizzato eseguire una delle operazioni seguenti:
     - Per aggiungere un nuovo criterio, selezionare **+ Crea**. Verrà avviata una procedura guidata per definire le impostazioni dei criteri.
     - Per modificare un criterio esistente, selezionarlo facendo clic sul nome del criterio. Nel riquadro a comparsa dei dettagli visualizzato selezionare **Modifica** nella **sezione Impostazioni di** protezione.
  4. Nella pagina **Impostazioni protezione** configurare le impostazioni seguenti:
     - Attiva **Selezionare l'azione per URL sconosciuti** potenzialmente dannosi nei messaggi .
     - Selezionare **Applica collegamenti sicuri ai messaggi inviati all'interno dell'organizzazione.**

  Per altre informazioni, vedi [Configurare i criteri Cassaforte collegamenti in Microsoft Defender per Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-safe-links-policies).
