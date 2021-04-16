---
title: Abilitare l'incorporamento delle finestre di dialogo legacy per aprire i report
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: c8a5634d5d79cbd584284b675e5db4e448a0d157
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814268"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>Abilitare l'incorporamento delle finestre di dialogo legacy per aprire i report

**Sintomo**

Gli utenti non possono aprire i report. “Si è verificato un errore. Controlla i dettagli tecnici per ulteriori informazioni.”

**Causa**

I report non riescono a caricarsi in UCI con l'errore "Il descrittore di modulo è nullo o non definito." I report in UCI richiedono ancora le finestre di dialogo legacy, pertanto il sistema del cliente deve avere *allowlegacydialogsembedding* abilitato.

**Soluzione**

1. Passare a **Impostazioni > Amministrazione > Impostazioni di sistema > Scheda generale**.

2. Impostare "Abilita incorporamento di alcune finestre di dialogo legacy nel client del browser delle interfacce unificate" su **Sì**.
