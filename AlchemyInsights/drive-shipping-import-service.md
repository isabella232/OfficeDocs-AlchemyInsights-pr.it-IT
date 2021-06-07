---
title: Spedizione unità nel servizio di importazione di Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11514"
- "9003046"
ms.openlocfilehash: 85d6e723e56b01fd9914165d8c9740f3b055947d
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 06/02/2021
ms.locfileid: "52721693"
---
# <a name="drive-shipping-in-the-microsoft-365-import-service"></a>Spedizione unità nel servizio di importazione di Microsoft 365

Utilizzare Spedizione unità copiando i file PST in un disco rigido e inviando poi tale disco rigido a Microsoft.

Per avviare il processo:

1. In **Governance delle informazioni** nel Centro conformità Microsoft 365, selezionare **Importa**.

1. Selezionare **Scegli tipo di processo di importazione**, quindi selezionare **Avanti**.

1. Per visualizzare i passaggi dell'opzione di importazione, selezionare **Spedizione dei dischi rigidi a una delle posizioni fisiche**.

Ecco alcuni aspetti da ricordare:

- Per importare file PST nelle cassette postali di Microsoft 365, è necessario avere il ruolo di importazione/esportazione di cassette postali in Exchange Online.
I file PST maggiori di 20 GB potrebbero influire sulle prestazioni.

- Sono supportate solo le unità SSD da 2,5 pollici o le unità disco rigido interno SATA II/III da 2,5 o 3,5 pollici.
Il disco rigido contenente i file PST deve essere crittografato con BitLocker.

- Il costo per l'importazione dei file PST nelle cassette postali di Microsoft 365 mediante la spedizione delle unità ammonta a $ 2 (dollari USA) per GB di dati.

Per ulteriori informazioni sull'uso del metodo Spedizione unità per l'importazione dei file PST, consultare [Utilizzare Spedizione unità per importare i file PST dell'organizzazione](/microsoft-365/compliance/use-drive-shipping-to-import-pst-files-to-office-365).