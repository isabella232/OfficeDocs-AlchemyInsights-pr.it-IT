---
title: Creare una relazione organizzativa per consentire agli utenti di collaborare con un'altra organizzazione
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
- "3800014"
- "898"
ms.openlocfilehash: b595fb87e18a055a7df1ff4c782a93591dd1f024
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816132"
---
# <a name="create-an-organization-relationship-to-allow-your-users-to-collaborate-with-another-organization"></a>Creare una relazione organizzativa per consentire agli utenti di collaborare con un'altra organizzazione

1. Dal dashboard dell'interfaccia di amministrazione di Microsoft 365, passare a **Amministrazione** > **Exchange**.
2. Passare a **organizzazione** > **condivisione**.
3. In **Condivisione tra organizzazioni** fare clic su **Nuovo** .
4. In **Nuova relazione organizzativa**, nella casella **Nome relazione**, digitare un nome amico per la relazione organizzativa.
5. Nella casella **Domini da condividere con**, digitare il dominio per l'organizzazione federata esterna di Exchange o Office 365 che si desidera configurare per la condivisione federata. Se necessario immettere più di un dominio, separare i nomi dei domini con una virgola. Ad esempio, contoso.com, service.contoso.com.
6. Selezionare la casella di controllo **Abilitare la condivisione delle informazioni di disponibilità calendario** per attivare la condivisione del calendario con i domini elencati. Impostare il livello di condivisione delle informazioni sulla disponibilità e impostare quale utente può condividerle.  

Per impostare il livello di accesso alle informazioni sulla disponibilità, selezionare una delle seguenti operazioni:

- **Informazioni sulla disponibilità in calendario, solo con data/ora**
- **Informazioni sulla disponibilità con ora, oggetto e posizione**  

 Per impostare quali utenti condivideranno le informazioni sulla disponibilità, selezionare una delle voci seguenti:

- **Tutti gli utenti dell'organizzazione**
- **Un gruppo di protezione specificato**  

Fare clic su **Sfoglia** per selezionare il gruppo di sicurezza da un elenco, fare clic su **ok**.

Fare clic su **Salva** per creare la relazione organizzativa.  

**Nota:** le configurazioni tra tenant non supportano la ricerca di informazioni sulla disponibilità tra i contatti personali. I contatti devono essere inclusi nell'elenco indirizzi globale per il funzionamento della la ricerca della disponibilità.

**Per informazioni complete su questo argomento, vedere:**

- [Creare una relazione dell'organizzazione in Exchange Online](https://docs.microsoft.com/exchange/sharing/organization-relationships/create-an-organization-relationship)
- [Modificare una relazione dell'organizzazione in Exchange Online](https://docs.microsoft.com/exchange/sharing/organization-relationships/modify-an-organization-relationship)
- [Rimuovere una relazione dell'organizzazione in Exchange Online](https://docs.microsoft.com/exchange/sharing/organization-relationships/remove-an-organization-relationship)
