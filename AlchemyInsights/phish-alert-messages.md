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
ms.openlocfilehash: ac4c157d6e202488659c56605768bbfd2b3af8e658d0a2f82e529fdac6763fa9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53999676"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Messaggi di posta elettronica di avviso dal criterio "Phish Delivered due to tenant or user override"

Un criterio di avviso predefinito denominato "Phish Delivered due to tenant or user override" è stato implementare ai tenant con Microsoft Defender per le licenze P1 e P2 Office 365. Se hai ricevuto questo avviso, ecco i passaggi da analizzare:

1. Nel messaggio di avviso fare clic **su** Visualizza avviso per passare alla **pagina Avvisi** nel Centro sicurezza & conformità.

2. Seleziona l'avviso per visualizzare l'opzione **Visualizza elenco messaggi** o Visualizza messaggi in Esplora **risorse.** Entrambe queste opzioni visualizzano i dettagli del messaggio, che include l'ID messaggio. Tieni presente che il collegamento Esplora minacce filtra automaticamente i messaggi che soddisfano i criteri di avviso. Potrebbe essere necessario modificare il filtro data in Threat Explorer.

Il messaggio di phishing è stato recapitato a causa di una sostituzione configurata manualmente:

- Mittente o dominio consentito impostato dall'utente.

- Un mittente o un dominio consentito impostato dall'amministratore in un criterio di protezione da posta indesiderata.

- Un indirizzo IP consentito in un criterio filtro connessioni.

- Una regola del flusso di posta (nota anche come regola di trasporto) configurata per consentire l'ingresso dei messaggi.

Se si ritiene che il messaggio sia stato erroneamente contrassegnato come phish, utilizzare il Outlook componente aggiuntivo [Segnala](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) messaggio per inviare esempi di messaggi a Microsoft.
