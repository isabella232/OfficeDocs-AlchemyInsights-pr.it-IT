---
title: 2681 Attack Simulator in Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 07d7622c00074f7bd0d567185824db448f1eeef3
ms.sourcegitcommit: 7232b48bcd8bb9867d52a2f055a46ce76a58b8da
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/27/2019
ms.locfileid: "37305336"
---
# <a name="attack-simulator-in-office-365"></a>Simulatore di attacchi in Office 365

- Si sta perdendo il simulatore d'attacco? Attack Simulator richiede **office 365 Advanced Threat Protection Plan 2 (ATP piano 2)** o **Office 365 Enterprise E5**. Simulatore di attacco **non** è incluso in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3 o qualsiasi abbonamento a Office 365 business.

- L'account utilizzato per avviare gli attacchi simulati richiede l'amministratore globale o le autorizzazioni di amministratore della sicurezza e l'autenticazione a più fattori (AMF). Per ulteriori informazioni sui requisiti dei simulatori di attacco, vedere [questo argomento](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).

- Aspetti importanti da sapere sulle simulazioni di attacchi di password per la **forza bruta** :

  - Se l'account di destinazione è abilitato per l'utilizzo dell'AMF e la password è stata indovinata, l'account non verrà visualizzato come compromesso (il secondo fattore di autenticazione sarà incompleto).

  - Il file della password non può essere superiore a 10 MB. Utilizzare una password per riga e includere una riga vuota (ritorno a capo) dopo l'ultima password dell'elenco.

- Aspetti importanti da sapere sulle simulazioni di attacchi di **phishing Spear** :

  - In base alla progettazione, non è possibile specificare un valore personalizzato per l' **URL del server di accesso di phishing**.

  - Se un destinatario utilizza il [componente aggiuntivo attiva messaggio di report](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) per segnalare il messaggio come phishing, potrebbe non essere possibile ricevere avvisi per il messaggio (poiché si tratta di un attacco simulato).

- Report: dopo aver completato l'attacco simulato, è possibile fare clic su **Dettagli attacco** per visualizzare il report.

- Per istruzioni dettagliate e nuove funzionalità in Attack Simulator, vedere [Attack Simulator in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
