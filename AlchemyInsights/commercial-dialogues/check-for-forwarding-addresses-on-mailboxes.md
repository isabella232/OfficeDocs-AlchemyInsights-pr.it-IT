---
title: Verificare la presenza di indirizzi di inoltro nelle cassette postali
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: a67305ed92e181f0ddfc5a929e8fe9631ceefdc99dea34118bc99975461f3868
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005814"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a>Verificare la presenza di indirizzi di inoltro nelle cassette postali

A volte gli hacker inoltrano i messaggi di posta elettronica degli utenti a se stessi, quindi prima di tutto verrà verificata la presenza di indirizzi di inoltro e regole sulla cassetta postale. Verificheremo quindi i log di controllo. Ecco come verificare la presenza di indirizzi di inoltro:

1. Selezionare **Utenti**  >  **Utenti attivi**.
1. Selezionare l'utente il cui account è stato compromesso.
1. Nel riquadro a comparsa visualizzato espandere **Mail Impostazioni** e quindi fare clic **su Edit** for **Email forwarding**.
1. Rimuovere gli indirizzi di inoltro non riconosciti.