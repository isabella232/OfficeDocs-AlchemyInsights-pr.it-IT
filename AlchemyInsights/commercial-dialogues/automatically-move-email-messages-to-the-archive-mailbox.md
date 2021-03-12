---
title: Spostare automaticamente i messaggi di posta elettronica nella cassetta postale di archiviazione
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
- "3100008"
- "7217"
ms.openlocfilehash: 14ded561ee2b3c244fadbdab42fd0e833a1c66d5
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736777"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a>Spostare automaticamente i messaggi di posta elettronica nella cassetta postale di archiviazione

Ecco come configurare un criterio per spostare automaticamente il vecchio messaggio di posta elettronica di un utente nella cassetta postale di archiviazione:

1. Passare a [**Sicurezza & governance dei**](https://go.microsoft.com/fwlink/p/?linkid=2077143)dati di conformità Archivio per verificare che sia stata abilitata una cassetta postale di archiviazione per  >    >   l'utente. In caso contrario, fare clic su **Abilita** e **quindi su Sì** nella casella di avviso.
2. Passare [**all'interfaccia di amministrazione di Exchange > gestione della conformità > tag di conservazione**](https://go.microsoft.com/fwlink/?linkid=2059104).
3. Scegliere l'icona + e quindi applica **automaticamente all'intera cassetta postale.**
4. Assegnare un nome al tag di conservazione e scegliere **Sposta in archivio**. Per il periodo di conservazione, immettere il tempo desiderato, ad esempio 90 giorni. Fare clic su **Salva**.
5. Ora crea un criterio di conservazione: scegli **i criteri di conservazione,** scegli l'icona per aggiungere un nuovo criterio.
6. Assegna un nome al criterio di conservazione, quindi fai clic e scorri per trovare e aggiungere il tag di conservazione appena creato. Fare clic su **Salva**.
7. Infine, applicare il criterio di conservazione alla cassetta postale dell'utente: ancora nell'interfaccia di amministrazione di Exchange, andare a **destinatari cassette**  >  **postali**. Scegli tutti gli utenti a cui vuoi applicare il criterio, quindi scegli **Modifica** (icona a forma di matita).
8. Nella finestra di dialogo fare clic su **Funzionalità cassetta postale**. In **Criteri di conservazione** applica il criterio appena creato > **Salva.**
9. Per istruzioni sull'applicazione del criterio a tutti gli utenti, vedere [Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).
