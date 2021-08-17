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
ms.openlocfilehash: 14a5a18bc1422572db567c9533fefe5a7e0120afd64df4a64623038cc063ce93
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058654"
---
# <a name="find-events-performed-on-inbox-rules"></a>Trovare gli eventi eseguiti sulle regole di Posta in arrivo

Quando le regole della posta in arrivo vengono create, modificate o eliminate, gli eventi vengono registrati nel registro di controllo. Ecco come esaminarli:

1. Passare al Centro [Office 365 sicurezza & conformità](https://go.microsoft.com/fwlink/p/?linkid=2077143).
1. Selezionare Ricerca > Ricerca log di controllo.

    > [!NOTE]
    > Se viene visualizzato un avviso che indica che è necessario attivare il controllo, procedere e attivarlo ora. Se questa funzionalità non è attivata, i risultati della ricerca non saranno in grado di estrarre i dati dalle date precedenti.
1. Selezionare il campo Attività e individuare Exchange delle cassette postali, quindi selezionare New-InboxRule Crea regola posta in arrivo da Outlook Web App. Al termine, fare clic all'esterno del riquadro per ridurre a icona il riquadro Attività.
1. Specificare l'intervallo di date e quindi nel campo Utenti selezionare il nome utente per l'utente che si desidera analizzare. È possibile selezionare più di un utente alla volta.
1. Selezionare Cerca. Le attività vengono visualizzate in Risultati.
1. Per visualizzare i dettagli, selezionare un'attività e quindi selezionare Altre informazioni. Nella sezione Parametri è possibile visualizzare il nome della regola, il set di condizioni e le azioni che verranno eseguite dalla regola.

Per ulteriori informazioni, vedere Search the Office 365 audit log to troubleshoot common scenarios.