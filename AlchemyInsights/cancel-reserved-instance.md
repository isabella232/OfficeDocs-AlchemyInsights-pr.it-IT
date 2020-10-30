---
title: Annullamento delle prenotazioni
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
- "9003552"
- "6817"
ms.openlocfilehash: 04875e33f07c6d0a4306b3579ef81f2d28c7f506
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 10/28/2020
ms.locfileid: "48791481"
---
# <a name="cancelling-reservation"></a>Annullamento delle prenotazioni

- **Modalità self-service:** è possibile annullare o cambiare un'istanza prenotata usando il [portale di Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Selezionare la prenotazione e fare clic su Rimborso o Cambio. Tenere presente che è necessario avere accesso come proprietario all'Ordine di prenotazione per chiederne il cambio o il rimborso. Se si dispone solo dell'accesso alla prenotazione non è possibile procedere con il rimborso o il cambio. Rivolgersi al proprietario dell'Ordine di prenotazione per chiedere l'assegnazione dell'accesso come proprietario della prenotazione.
- **Criteri di cambio:** è possibile cambiare la prenotazione con un'altra dello stesso tipo. Non verranno applicate **penali** per il cambio. L'impegno complessivo per una nuova prenotazione deve essere maggiore della somma dell'ammontare del rimborso della prenotazione cambiata e dei pagamenti mensili futuri, se applicabili.
- **Politica di rimborso:** la somma dei rimborsi e dei pagamenti futuri annullati non può essere superiore a 50.000 USD in una finestra di fatturazione di 12 mesi. **Al momento non viene addebitata alcuna penalità** sui rimborsi, ma potrebbe cambiare in futuro.  
    **Eccezioni:** le funzionalità di cambio e annullamento in modalità self-service non sono disponibili per i clienti con Contratto Enterprise US Government.
- Il supporto **API/PS/CLI** non è disponibile per gli [annullamenti e rimborsi in modalità self service per le prenotazioni di Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support).
- Le funzionalità di cambio e annullamento in modalità self-service non sono disponibili per i clienti con Contratto Enterprise US Government. Altri tipi di sottoscrizione US Government, tra cui Pagamento a consumo e CSP, sono supportati

Altre informazioni: [Come vengono elaborate le transazioni relative a rimborsi e cambi](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)  
Altre informazioni: [Criteri di rimborso e di cambio](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)  
Per altre domande: [consultare i documenti sulle istanze riservate](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Cambio di un'istanza riservata esistente (in modalità self-service)**

È possibile cambiare la prenotazione in un'altra dello stesso tipo. Se non è più necessaria, è anche possibile ottenere il rimborso di una prenotazione fino a un massimo di 50.000 USD all'anno. Le funzionalità di cambio e annullamento in modalità self-service non sono disponibili per i clienti con Contratto Enterprise US Government. Altri tipi di sottoscrizione US Government, tra cui Pagamento a consumo e CSP, sono supportati. È necessario avere l'accesso come proprietario all'Ordine di prenotazione per chiedere il cambio o il rimborso di una prenotazione esistente.

La procedura seguente illustra come completare la transazione.

1. Accedere al [Portale di Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Selezionare le prenotazioni che di cui si vuole il rimborso e fare clic su **Cambio**
2. Selezionare il prodotto VM che si vuole acquistare e digitare la quantità. Verificare che l'ammontare del nuovo acquisto sia maggiore del totale del rimborso, vedere [Determinare le dimensioni appropriate prima dell'acquisto](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3. Rivedere e completare la transazione

**Rimborso di un'istanza riservata**

Per ottenere il rimborso di una prenotazione, passare a **Dettagli della prenotazione** e quindi fare clic su **Rimborso**

**Rimborso proporzionale:**

**Esempi di requisiti proporzionali e minimi di rimborso o cambio**  
Esempio di prenotazione anticipata:

- Si acquista un'istanza riservata di un anno per $120 il 1° gennaio
- Il 7 aprile si vuole ottenere il rimborso o cambiare la prenotazione
- Poiché si è usufruito della prenotazione per 97 giorni, si otterrà un rimborso di: (1-97/365) x $120. (ossia $88,1). Al momento non si applicano penalità sui rimborsi
- In caso di cambio, il nuovo acquisto deve essere maggiore di $88,1
- Al momento non si applicano penalità sui rimborsi

**Esempio di prenotazione di un piano di fatturazione:**

- Si acquista un'istanza riservata di un anno per $10 al mese
- Il 7 aprile si vuole ottenere il rimborso o cambiare la prenotazione
- Poiché l'ultimo pagamento è stato effettuato 7 giorni prima, si otterrà un rimborso di: (1-7/31) x $10. (ossia $7,74).
- I pagamenti futuri annullati ammontano a $80. Al momento non si applicano penalità sui rimborsi
- Questo annullamento detrae $87,74 dal limite di rimborso annuale di $50.000
- In caso di cambio, il valore totale del nuovo acquisto deve essere superiore a $87,74

**Documenti consigliati**

- [Come vengono elaborate le transazioni relative a rimborsi e cambi](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)
- [Criteri di rimborso e cambio](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)