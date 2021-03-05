---
title: Trovare gli eventi eseguiti sulle regole di Posta in arrivo
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: deb83d278a2b398b4ea6fc31b043c33309b736e3
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/05/2021
ms.locfileid: "50465001"
---
# <a name="find-events-performed-on-inbox-rules"></a>Trovare gli eventi eseguiti sulle regole di Posta in arrivo

Quando le regole di Posta in arrivo vengono create, modificate o eliminate, gli eventi vengono registrati nel registro di controllo. Ecco come esaminarli:

1. Passare al Centro sicurezza e conformità di [Office 365 &.](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. Selezionare Ricerca > ricerca nel log di controllo.

    > [!NOTE]
    > Se viene visualizzato un avviso che indica che è necessario attivare il controllo, procedere e attivarlo ora. Se questa funzionalità non è attivata, i risultati della ricerca non saranno in grado di estrarre i dati dalle date precedenti.
1. Selezionare il campo Attività e trovare le attività della cassetta postale di Exchange, quindi selezionare New-InboxRule Crea regola posta in arrivo da Outlook Web App. Al termine, fare clic all'esterno del riquadro per ridurre a icona il riquadro Attività.
1. Specificare l'intervallo di date e quindi nel campo Utenti selezionare il nome utente per l'utente che si desidera analizzare. È possibile selezionare più di un utente alla volta.
1. Selezionare Cerca. Le attività vengono visualizzate in Risultati.
1. Per visualizzare i dettagli, selezionare un'attività e quindi selezionare Altre informazioni. Nella sezione Parametri è possibile visualizzare il nome della regola, le condizioni impostate e le azioni che verranno eseguite dalla regola.

Per ulteriori informazioni, vedere Eseguire una ricerca nel log di controllo di Office 365 per risolvere i problemi relativi agli scenari comuni.