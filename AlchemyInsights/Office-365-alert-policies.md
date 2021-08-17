---
title: 1385-Office-365-alert-policies
ms.author: markjjo
author: markjjo
manager: lauraw
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1385"
- "3200002"
ms.assetid: ''
ms.openlocfilehash: 681f7609f32b004ddfa7bfbeff179757e7063657
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58312691"
---
# <a name="alert-policies"></a>Criteri di avviso

Microsoft 365 contiene i [](https://docs.microsoft.com/microsoft-365/compliance/alert-policies#default-alert-policies) criteri di avviso predefiniti che attivano gli avvisi per le organizzazioni con una sottoscrizione Microsoft 365 Enterprise o Microsoft 365 US Government E1/G1, E3/G3 o E5/G5. Pertanto, gli amministratori possono ricevere una notifica tramite posta elettronica di avviso inviata da Office365Alerts@microsoft.com con una riga dell'oggetto, ad esempio "Avviso di gravità bassa: nome del criterio *di avviso".* Le notifiche di avviso vengono inviate quando vengono attivati avvisi per attività comuni, ad esempio quando gli utenti:

- Creare regole di Posta in arrivo che inoltrano la posta elettronica.
- Assegnare le autorizzazioni alla cassetta postale.
- Condividere o eliminare un numero elevato di file nella condivisione SharePoint file.
- Creare ricerche eDiscovery ed esportare i risultati della ricerca.

Per esaminare e agire su un avviso:

1. Eseguire uno dei seguenti passaggi:
   - Nell'Centro conformità Microsoft 365 <https://compliance.microsoft.com> in , passare a **Avvisi**. In caso contrario, per passare direttamente alla **pagina Avvisi,** utilizzare <https://compliance.microsoft.com/compliancealerts> .
   - Nel portale Microsoft 365 Defender , passare a Eventi imprevisti <https://security.microsoft.com> **&** \> **avvisi**. In caso contrario, per passare direttamente alla **pagina Avvisi,** utilizzare <https://security.microsoft.com/alerts> .
2. Fare clic su un avviso per visualizzare una pagina a comparsa con informazioni sull'avviso.

È possibile eseguire un'azione su un avviso, ad esempio rimuovere una regola di posta in arrivo [sospetta.](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account) Oppure puoi semplicemente chiudere l'avviso facendo clic **su Risolvi** nella pagina a comparsa dell'avviso.

Per ulteriori informazioni sulla configurazione e sulla gestione dei criteri di avviso, vedere [questo articolo.](https://docs.microsoft.com/microsoft-365/compliance/alert-policies)

**Importante:** le notifiche tramite posta elettronica di avviso di Microsoft non ti chiederanno mai di eseguire le operazioni seguenti:

- Fornire una password
- Verificare i dettagli di sicurezza dell'account
- Eseguire di nuovo l'autenticazione

Se si riceve un messaggio di posta elettronica con questo tipo di richieste, non è stato inviato da Microsoft e deve essere considerato un tentativo di phishing. Se si riceve un messaggio con questo tipo di richieste, [segnalare il messaggio a Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-messages-to-microsoft).
