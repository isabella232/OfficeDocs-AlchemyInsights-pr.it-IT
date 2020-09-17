---
title: Creare un criterio di condivisione per consentire agli utenti di condividere il proprio calendario con utenti esterni all'organizzazione.
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 9ece122e0905d1afeb26e50fa0a5e049eee5c09d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806727"
---
# <a name="create-a-sharing-policy-to-allow-your-users-to-share-their-calendar-with-people-outside-your-organization"></a>Creare un criterio di condivisione per consentire agli utenti di condividere il proprio calendario con utenti esterni all'organizzazione.

1. Dal dashboard dell'interfaccia di amministrazione di Microsoft 365, passare a **Amministrazione** > **Exchange**.
2. Passare a **organizzazione** > **condivisione**.
3. Nella visualizzazione elenco, sotto **Condivisione individuale** fare clic su **Nuovo** .
4. In **nuovi criteri di condivisione** digitare il nome descrittivo per il criterio di condivisione nella casella **Nome criteri**.
5. Fare clic su **Aggiungi** per definire le regole di condivisione per il criterio.
6. In **regola di condivisione** selezionare uno dei seguenti pulsanti di opzione per specificare i domini per la condivisione:
    - **Condivisione con tutti i domini**
    - **Condivisione con uno specifico dominio**
8. Se è stato selezionato **Condivisione con uno specifico dominio**, digitare il dominio per la condivisione. Se è necessario inserire più di un dominio per il criterio di condivisione, salvare le impostazioni del primo dominio, quindi modificare le regole di condivisione al fine di aggiungervi ulteriori domini.
9. Per specificare le informazioni che possono essere condivise, selezionare la casella di controllo **Condividi la tua cartella del calendario**, quindi selezionare una delle seguenti opzioni:
    - **Informazioni sulla disponibilità in calendario, solo con data/ora**
    - **Informazioni sulla disponibilità in calendario, con data/ora, oggetto e luogo**
    - **Tutte le informazioni di calendario sull'appuntamento, incluse ora, oggetto, posizione e titolo**
11. Fare clic su **salva** per impostare le regole per il criterio di condivisione.
12. Per impostare questo criterio come il nuovo criterio di condivisione predefinito per gli utenti nell'organizzazione, selezionare la casella di controllo **Imposta questi criteri come predefiniti per la condivisione**.
13. Fare clic su **Salva** per creare il criterio di condivisione.  

**Per informazioni complete su questo argomento, vedere:**

- [Creare un criterio di condivisione in Exchange Online](https://docs.microsoft.com/exchange/sharing/sharing-policies/create-a-sharing-policy)
- [Applicare un criterio di condivisione alle cassette postali in Exchange Online](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy)
- [Modificare, disabilitare o rimuovere un criterio di condivisione in Exchange Online](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)