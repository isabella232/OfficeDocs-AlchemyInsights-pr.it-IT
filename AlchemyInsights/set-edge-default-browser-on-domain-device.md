---
title: Impostare Microsoft Edge come browser predefinito su un dispositivo aggiunto a un dominio
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: f51a455ea15b7bd92f548f2c1717be9888b43d07
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426838"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-domain-joined-device"></a>Impostare Microsoft Edge come browser predefinito su un dispositivo aggiunto a un dominio

Impostare Microsoft Edge come browser predefinito: 

1. [Crea file di configurazione delle associazioni predefinite](https://go.microsoft.com/fwlink/?linkid=2132437) e archiviarlo localmente o in una condivisione di rete.

1. Aprire l'editor Criteri di gruppo e passare a **Configurazione computer** > **Modelli amministrativi** > **Componenti di Windows** > **Esplora file**.

1. Selezionare **Imposta file di configurazione delle associazioni predefinite**.

1. Selezionare **Impostazioni criterio**, quindi **Abilitato**.

1. In **Opzioni**, immettere la posizione del file di configurazione delle associazioni predefinite, quindi selezionare **OK**.
