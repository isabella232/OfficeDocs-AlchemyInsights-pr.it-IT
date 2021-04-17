---
title: Fatturazione per l'acquisto di istanze riservate
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6814"
- "9003552"
ms.openlocfilehash: 9d71554d2089a6d9e5d4850149d113959f3d43c0
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820326"
---
# <a name="billing-for-reserved-instance-purchase"></a>Fatturazione per l'acquisto di istanze riservate

L'acquisto dell'istanza riservata viene addebitato sulla modalità di pagamento associata alla sottoscrizione selezionata al momento dell'acquisto. Il tipo di sottoscrizione deve essere un contratto enterprise (numero dell'offerta: MS-AZR-0017P), Pay-As-You-Go (numero dell'offerta: MS-AZR-0003P), Contratto per i clienti Microsoft o CSP.

- Per una sottoscrizione enterprise, gli addebiti vengono detratti dal saldo dell'impegno monetario della registrazione o addebitati come in evaso
- Per la sottoscrizione con pagamento in base al consumo, gli addebiti vengono fatturati alla carta di credito o al metodo di pagamento della fattura nell'abbonamento

**Annullamento della prenotazione**

- **Self-service:** Puoi annullare o scambiare manualmente un'istanza riservata usando [il portale di Azure.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) Seleziona la prenotazione e fai clic su rimborso o cambio. Tieni presente che devi disporre dell'accesso proprietario nell'ordine di prenotazione per lo scambio o il rimborso. L'accesso solo alla prenotazione non consente di procedere con il rimborso o lo scambio. Chiedere al proprietario dell'ordine di prenotazione di fornire al proprietario l'accesso all'ordine di prenotazione
- **Criteri di Exchange:** È possibile scambiare una prenotazione per un'altra prenotazione dello stesso tipo: non sono previste **sanzioni per** lo scambio di prenotazioni. L'impegno totale con una nuova prenotazione deve essere maggiore della somma dell'importo del rimborso della prenotazione scambiata e dei futuri pagamenti mensili (se applicabile)
- **Criteri di rimborso:** La somma del rimborso e dei pagamenti futuri annullati non può superare i $50.000 USD in una finestra di rotolamento di 12 mesi. Al momento **non viene addebitata alcuna penalità** per i rimborsi, ma potrebbe essere addebitata sui rimborsi futuri

**Eccezioni:** La funzionalità di scambio e annullamento self-service non è disponibile per i Contratto Enterprise statunitensi

- **Il supporto API/PS/CLI** non è disponibile per l'annullamento e i rimborsi per gli scambi [self-service](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support) e i rimborsi per prenotazioni di Azure
- La funzionalità di scambio e annullamento self-service non è disponibile per i Contratto Enterprise statunitensi. Sono supportati altri tipi di abbonamento us government, tra cui Pay-As-You-Go e CSP

Ulteriori informazioni : [Come vengono elaborate le](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) transazioni di restituzione e cambio Ulteriori informazioni : Criteri di Exchange e [rimborso](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) Altre domande: [Visitare i documenti di istanza riservati](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Exchange un'istanza riservata esistente (self-service)**

È possibile scambiare una prenotazione per un'altra prenotazione dello stesso tipo. Puoi anche rimborsare una prenotazione, fino a $50.000 USD all'anno, se non è più necessaria. La funzionalità di scambio e annullamento self-service non è disponibile per i Contratto Enterprise statunitensi. Sono supportati altri tipi di sottoscrizione per enti pubblici statunitensi, tra cui Pay-As-You-Go e CSP. Devi disporre dell'accesso proprietario nell'ordine di prenotazione per scambiare o rimborsare una prenotazione esistente.

I passaggi seguenti illustrano la procedura per completare la transazione

1.Accedere al portale [di Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Selezionare le prenotazioni che si desidera rimborsare e fare clic su **Exchange** 2.Selezionare il prodotto vm che si desidera acquistare e digitare una quantità. Assicurati che il nuovo totale acquisti sia superiore al totale restituito [Determinare le dimensioni giuste prima di acquistare](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy).
3.Rivedere e completare la transazione

**Rimborso per un'istanza riservata**

Per rimborsare una prenotazione, vai a **Dettagli prenotazione e** fai clic su **Rimborso**

**Rimborso con tariffa pro:**

**Esempi di razione e requisito minimo per il rimborso e lo scambio** Esempio di prenotazione anticipata:

- Si acquista un periodo di un anno ri per $120 il 1 gennaio
- Il 7 aprile vuoi rimborsare o scambiare questa prenotazione
- Dal momento che la prenotazione è stata live per 97 giorni, si otterrà (1-97/365) * $120 indietro. (ad esempio $ 88,1). Al momento non è prevista alcuna penalità per i rimborsi
- In caso di scambio, il nuovo acquisto deve essere maggiore di $88,1
- Al momento non è prevista alcuna penalità per i rimborsi

**Esempio di prenotazione del piano di fatturazione:**

- Si acquista un periodo di un anno ri per $10 al mese
- Il 7 aprile vuoi rimborsare o scambiare questa prenotazione
- Poiché l'ultimo pagamento è avvenuto 7 giorni, si otterrà (1-7/31) * $10 indietro. (ad esempio $ 7,74)
- I pagamenti futuri annullati sono $ 80. Al momento non è prevista alcuna penalità per i rimborsi
- Questo annullamento detrarrà $ 87,74 dal limite di rimborso di $ 50.000
- In caso di scambio, il valore totale del nuovo acquisto deve essere maggiore di $87,74

**Impossibile visualizzare la fattura per l'ultimo periodo di fatturazione**

Alcuni dei possibili motivi per cui potrebbe non essere visualizzata una fattura:

- Hai un importo di credito mensile con l'abbonamento che non hai superato o hai una versione di valutazione gratuita. Una fattura viene generata solo quando si deve denaro
- Sono meno di 30 giorni dal giorno in cui hai effettuato la sottoscrizione ad Azure
- La fattura non è ancora stata generata. Attendere la fine del periodo di fatturazione
- Se non si è l'amministratore dell'account, le fatture precedenti potrebbero non essere disponibili

**Scaricare la fattura dal portale di Azure (.pdf)**

- Selezionare la sottoscrizione dalla pagina [Abbonamenti](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) nel portale di Azure [come utente con accesso alle fatture](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- Seleziona **fatture**
- Fare clic su **Scarica fattura** per visualizzare una copia della fattura in formato PDF. Se viene visualizzato **Non disponibile,** vedere Perché non viene visualizzata [una fattura per l'ultimo periodo di fatturazione?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

**Ricevere la fattura tramite posta elettronica (.pdf)**

- Seleziona l'abbonamento nella [pagina Abbonamenti.](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) Fai **clic su Fatture** e quindi invia una e-mail alla fattura
- Fai **clic su Acconsentire** esplicitamente e accettare le condizioni. Sarà necessario acconsentire esplicitamente a ogni sottoscrizione di cui si è proprietari

Nota: se non ricevi un messaggio di posta elettronica dopo aver seguito la procedura, assicurati che l'indirizzo di posta elettronica sia corretto nelle preferenze [di comunicazione nel profilo](https://account.windowsazure.com/profile)

**Scaricare i dati di utilizzo dal portale di Azure**

- Accedere al [Centro account di Azure](https://account.windowsazure.com/Subscriptions) come amministratore [dell'account](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- Selezionare l'abbonamento per il quale si desiderano le informazioni sulla fattura e sull'utilizzo
- Seleziona **cronologia fatturazione**
- Selezionare **Visualizza estratto conto** corrente per visualizzare una stima degli addebiti al momento della generazione della stima
- Selezionare **Scarica utilizzo** per scaricare i dati di utilizzo giornalieri come file CSV. Se sono disponibili due versioni, scaricare la versione 2

Altre domande: [Visitare i documenti delle istanze riservate](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Documenti consigliati**

- [Nozioni di base sulla fatturazione](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Comprendere come viene applicato lo sconto istanza riservata](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Scaricare o visualizzare la fattura di fatturazione di Azure e i dati di utilizzo giornalieri](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Comprendere come viene applicato lo sconto istanza riservata](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Informazioni sull'utilizzo dell'istanza riservata per la sottoscrizione con pagamento in base al consumo](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Informazioni sull'utilizzo dell'istanza riservata per la registrazione enterprise](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Costi software Windows non inclusi nelle istanze riservate](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Istanze riservate nel programma CSP (Partner Central Cloud Solution Provider)](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)