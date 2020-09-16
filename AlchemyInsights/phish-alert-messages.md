---
title: 2491 messaggi di posta elettronica di avviso provenienti dal criterio ' phishing recapitato a causa di override del tenant o dell'utente
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
ms.openlocfilehash: 5b5faa08542cb5878107f10afb34427f636562ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728615"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Avvisare i messaggi di posta elettronica dal criterio ' phishing recapitato a causa del tenant o dell'utente

Un criterio di avviso predefinito denominato "phishing recapitato a causa del tenant o dell'utente" è stato implementato nei tenant con Office 365 ATP P1 e P2 licenses. Se è stato ricevuto questo avviso, ecco i passaggi da eseguire per esaminare:

1. Dal messaggio di avviso, fare clic su **Visualizza avviso** per passare alla pagina **avvisi** nel centro sicurezza & conformità.

2. Selezionare l'avviso per visualizzare l'opzione per **visualizzare l'elenco** dei messaggi o visualizzare i messaggio **in Esplora**. Entrambe queste opzioni consentono di utilizzare i dettagli del messaggio, che include l'ID del messaggio. Si noti che il collegamento Esplora minacce filtra automaticamente i messaggi che corrispondono ai criteri di avviso. Potrebbe essere necessario modificare il filtro data in Esplora minacce.

Il messaggio di phishing è stato recapitato a causa di una sostituzione configurata manualmente:

- Un mittente o un dominio consentito impostato dall'utente.

- Un mittente o un dominio consentito impostato dall'amministratore in un criterio di protezione da posta indesiderata.

- Un indirizzo IP consentito in un criterio di filtro delle connessioni.

- Regola del flusso di posta (nota anche come regola di trasporto) configurata per consentire l'utilizzo dei messaggi.

Se si ritiene che il messaggio sia stato contrassegnato erroneamente come phishing, utilizzare il [componente aggiuntivo dei messaggi del rapporto](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) di Outlook per inviare esempi di messaggi a Microsoft.
