---
title: Inventario software mancante o non corretto
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11382"
- "9001470"
ms.openlocfilehash: e886a53f8c063b5395dd002a7d16186985584d72
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 05/26/2021
ms.locfileid: "52658052"
---
# <a name="software-inventory-is-missing-or-inaccurate"></a>Inventario software mancante o non corretto

L'inventario software nella funzionalità per la gestione di minacce e vulnerabilità è un elenco di software noti dell'organizzazione con enumerazioni CPE ( Common Platform Enumeration) ufficiali.

I prodotti software senza CPE ufficiale non hanno vulnerabilità pubblicate. L'inventario include anche dettagli come il nome del fornitore, il numero di punti deboli, le minacce e il numero di dispositivi esposti.

Le modifiche al software nei dispositivi vengono in genere rispecchiate portali di sicurezza entro due ore. A volte, tuttavia, può essere necessario più tempo. Attualmente non è possibile forzare una sincronizzazione, la valutazione è continua.

Se è stata apportata una modifica al software e la modifica non è rispecchiata in modo accurato in TVM dopo 5 ore, seguire questa procedura:

1. Consultare la sezione delle prove software per capire come è stato rilevato il software.
1. Assicurarsi che il software sia supportato. Il software può essere visibile solo a livello di dispositivo, anche se attualmente non è supportato dalla gestione di minacce e vulnerabilità. Tuttavia, sono disponibili solo dati limitati.
1. Per la procedura da seguire per segnalare l'imprecisione del portale, vedere [Imprecisione dei report](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).
   
    **Nota**: la segnalazione di un'inesattezza dal portale MDE è un canale di comunicazione con i tecnici unidirezionale. Se il problema è urgente, aprire un ticket di supporto.

Per ulteriori informazioni, vedere [Inventario software: gestione di minacce e vulnerabilità](/microsoft-365/security/defender-endpoint/tvm-software-inventory).