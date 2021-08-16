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
ms.openlocfilehash: b173c6eb3bbbd1beba3b59878ae12bbe7684d0447a16fef746e5b97b82349e53
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54065288"
---
# <a name="attack-simulator-in-microsoft-365"></a>Simulatore di attacco in Microsoft 365

- Simulatore di attacco mancante? Attack Simulator richiede **Microsoft Defender per Office 365 Piano 2** o Office 365 Enterprise **E5.** Il simulatore **di attacco** non è incluso in Microsoft Defender per Office 365 Piano 1, Office 365 Enterprise E3 o in Microsoft 365 Apps for business abbonamenti.

- L'account utilizzato per avviare attacchi simulati richiede autorizzazioni di amministratore globale o amministratore della sicurezza e autenticazione a più fattori (MFA). Per ulteriori informazioni sui requisiti del simulatore di attacco, vedere [questo argomento.](/microsoft-365/security/office-365-security/attack-simulator)

- Aspetti importanti da sapere sulle simulazioni di attacco **Brute Force Password:**

  - Se l'account di destinazione ha la MFA abilitata e la password è stata indovinata correttamente, l'account non verrà visualizzato come compromesso (il secondo fattore di autenticazione sarà incompleto).

  - Il file delle password non può essere superiore a 10 MB. Utilizzare una password per riga e includere una riga vuota (ritorno a capo) dopo l'ultima password nell'elenco.

- Aspetti importanti da sapere sulle **simulazioni di attacco spear phishing:**

  - Per impostazione predefinita, non è possibile fornire un valore personalizzato per l'URL del **server di accesso phishing.**

  - Se un destinatario utilizza il componente aggiuntivo Segnala messaggio per segnalare il messaggio come phishing, è possibile che non si ricevano avvisi per il messaggio (perché si tratta di un attacco simulato). [](/microsoft-365/security/office-365-security/enable-the-report-message-add-in)

- Report: al termine dell'attacco simulato, è possibile fare clic su **Dettagli attacco** per visualizzare il report.

- Per istruzioni dettagliate e nuove funzionalità in Attack Simulator, vedi [Simulatore](/microsoft-365/security/office-365-security/attack-simulator)di attacco in Microsoft 365 .
