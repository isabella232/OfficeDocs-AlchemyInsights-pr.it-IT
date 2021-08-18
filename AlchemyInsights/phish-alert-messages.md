---
title: 2491 Avvisa i messaggi di posta elettronica dal criterio "Phish Delivered due to tenant or user override"
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 90b078147bbb1e60cba0a2de6e49a862469f93aa
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316362"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Messaggi di posta elettronica di avviso dal criterio "Phish Delivered due to tenant or user override"

Un criterio di avviso predefinito denominato **Phish Delivered a** causa della sostituzione del tenant o dell'utente è disponibile nelle organizzazioni con Microsoft Defender per Office 365 licenze P1 e P2. Se hai ricevuto questo avviso, ecco i passaggi da analizzare:

1. Nel messaggio di avviso fare clic **su Visualizza** avviso per passare alla **pagina Avvisi** nel Microsoft 365 Defender portale.

2. Seleziona l'avviso per visualizzare l'opzione **Visualizza elenco messaggi** o Visualizza messaggi in Esplora **risorse.** Entrambe queste opzioni visualizzano i dettagli del messaggio, che include l'ID messaggio. Tieni presente che il collegamento Esplora minacce filtra automaticamente i messaggi che soddisfano i criteri di avviso. Potrebbe essere necessario modificare il filtro data in Threat Explorer.

Il messaggio di phishing è stato recapitato a causa di una sostituzione configurata manualmente:

- Mittente o dominio consentito impostato dall'utente.
- Un mittente o un dominio consentito impostato dall'amministratore in un criterio di protezione da posta indesiderata.
- Un indirizzo IP consentito in un criterio filtro connessioni.
- Una regola del flusso di posta (nota anche come regola di trasporto) configurata per consentire l'ingresso dei messaggi.

Se si ritiene che il messaggio sia stato erroneamente contrassegnato come phishing, utilizzare l'invio [dell'amministratore](https://docs.microsoft.com/microsoft-365/security/office-365-security/admin-submission) per segnalare il messaggio a Microsoft.

Gli utenti possono utilizzare il componente aggiuntivo Segnala messaggio o il componente aggiuntivo Segnala [phishing](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) Outlook inviare esempi di messaggi a Microsoft.
