---
title: Consentire o disabilitare un video IP in Teams
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
- "9002537"
- "5617"
ms.openlocfilehash: ad60225e5deee4a37831a3145d37916c9ce849f9f4cf475dce4c9a6210f83af9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940643"
---
# <a name="teams-allow-or-disable-ip-video"></a>Consentire o disabilitare un video IP in Teams

**Cambiare o creare un criterio di riunione**

Per modificare o creare un criterio riunione, passare **all'interfaccia di amministrazione di Microsoft Teams > Riunioni > Criteri di riunione**. Selezionare un criterio dall'elenco o fare clic su **Aggiungi**. Se si sta creando un nuovo criterio, aggiungere un nome e una descrizione. Il nome non può contenere caratteri speciali o più di 64 caratteri. Scegliere le impostazioni desiderate e poi fare clic su **Salva**.

Ad esempio, si supponga di avere molti utenti e di voler limitare la larghezza di banda necessaria per la riunione. È possibile creare un nuovo criterio personalizzato denominato "Larghezza di banda limitata" e disabilitare le impostazioni seguenti:

In **Audio e video**:

- Disattivare Consenti registrazione cloud.
- Disattivare Consenti video IP.

Assegnare poi il criterio agli utenti.

**Assegnare un criterio riunione agli utenti**

1. Nel riquadro di spostamento sinistro dell'interfaccia di amministrazione di Microsoft Teams passare a **Utenti** e quindi fare clic sull'utente.
2. Per selezionare l'utente facendo clic a sinistra del nome utente e poi fare clic su **Impostazioni di modifica**.
3. In **Criteri riunioni** selezionare il criterio da assegnare e poi fare clic su **Applica**.

Per altre informazioni, vedere [Gestire i criteri di riunione in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).
