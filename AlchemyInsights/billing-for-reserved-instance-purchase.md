---
title: Fatturazione per l’acquisto dell’istanza riservata
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6814"
- "9003552"
ms.openlocfilehash: 6cdcb5af27a475cc838eb434ff025eb18356360c
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 10/30/2020
ms.locfileid: "48816007"
---
# <a name="billing-for-reserved-instance-purchase"></a>Fatturazione per l’acquisto dell’istanza riservata

L'acquisto dell’istanza riservata viene addebitato sulla modalità di pagamento associata all'abbonamento selezionato al momento dell'acquisto. Il tipo di abbonamento deve essere un contratto Enterprise (numero offerta: MS-AZR-0017P), con pagamento in base al consumo (numero offerta: MS-AZR-0003P), un Contratto del cliente Microsoft o Microsoft Cloud Solution Provider.

- Per gli abbonamenti Enterprise, gli addebiti vengono detratti dal saldo dell’impegno monetario al momento della registrazione o addebitati come eccedenza
- Per gli abbonamenti con pagamento in base al consumo, gli addebiti vengono intestati alla carta di credito o alla modalità di pagamento delle fatture dell'abbonamento

**Annullamento delle prenotazioni**

- **Modalità self-service:** è possibile annullare o cambiare un'istanza prenotata usando il [portale di Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Selezionare la prenotazione e fare clic su Rimborso o Cambio. Tenere presente che è necessario avere accesso come proprietario all'Ordine di prenotazione per chiederne il cambio o il rimborso. Se si dispone solo dell'accesso alla prenotazione non è possibile procedere con il rimborso o il cambio. Rivolgersi al proprietario dell'Ordine di prenotazione per chiedere l'assegnazione dell'accesso come proprietario della prenotazione.
- **Criteri di cambio:** è possibile cambiare la prenotazione con un'altra dello stesso tipo. Non verranno applicate **penali** per il cambio. L'impegno complessivo per una nuova prenotazione deve essere maggiore della somma dell'ammontare del rimborso della prenotazione cambiata e dei pagamenti mensili futuri, se applicabili.
- **Politica di rimborso:** la somma dei rimborsi e dei pagamenti futuri annullati non può essere superiore a 50.000 USD in una finestra di fatturazione di 12 mesi. **Al momento non viene addebitata alcuna penalità** sui rimborsi, ma potrebbe cambiare in futuro.

**Eccezioni:** le funzionalità di cambio e annullamento in modalità self-service non sono disponibili per i clienti con Contratto Enterprise US Government.

- Il supporto **API/PS/CLI** non è disponibile per gli [annullamenti e rimborsi in modalità self service per le prenotazioni di Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support).
- Le funzionalità di cambio e annullamento in modalità self-service non sono disponibili per i clienti con Contratto Enterprise US Government. Altri tipi di sottoscrizione US Government, tra cui Pagamento a consumo e CSP, sono supportati

Per ulteriori informazioni, vedere [come vengono elaborate le transazioni di invio e di Exchange](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) ulteriori informazioni: [criteri di Exchange e di rimborso](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) altre domande: [visita l'istanza riservata documenti](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Cambio di un'istanza riservata esistente (in modalità self-service)**

È possibile cambiare la prenotazione in un'altra dello stesso tipo. Se non è più necessaria, è anche possibile ottenere il rimborso di una prenotazione fino a un massimo di 50.000 USD all'anno. Le funzionalità di cambio e annullamento in modalità self-service non sono disponibili per i clienti con Contratto Enterprise US Government. Altri tipi di sottoscrizione US Government, tra cui Pagamento a consumo e CSP, sono supportati. È necessario avere l'accesso come proprietario all'Ordine di prenotazione per chiedere il cambio o il rimborso di una prenotazione esistente.

La procedura seguente illustra come completare la transazione.

1. accedere al portale di [Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Selezionare le prenotazioni che si desidera rimborsare e fare clic su **Exchange** 2. Selezionare il prodotto VM che si desidera acquistare e digitare una quantità. Verificare che il nuovo totale di acquisto sia superiore a quello restituito per [determinare la dimensione corretta prima dell'acquisto](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy).
3. Revisione e completamento della transazione

**Rimborso di un'istanza riservata**

Per ottenere il rimborso di una prenotazione, passare a **Dettagli della prenotazione** e quindi fare clic su **Rimborso**

**Rimborso proporzionale:**

**Esempi di requisiti di Pro-razione e minimi per rimborsi ed Exchange** Esempio di prenotazione upfront:

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

**Impossibile visualizzare la fattura per l'ultimo periodo di fatturazione**

Alcuni possibili motivi per cui potrebbe non essere visualizzata una fattura:

- Si dispone di un importo mensile di credito con l'abbonamento che non è stato superato o che si dispone di una versione di valutazione gratuita. Una fattura viene generata solo quando si deve denaro
- Ha meno di 30 giorni dal giorno in cui è stato sottoscritto Azure
- La fattura non è ancora stata generata. Attendi fino alla fine del periodo di fatturazione
- Se non si è l'amministratore dell'account, le fatture meno recenti potrebbero non essere disponibili

**Scaricare la fattura dal portale di Azure (. pdf)**

- Selezionare l'abbonamento dalla pagina [abbonamenti](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) in Azure Portal come [utente con accesso alle fatture](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- Selezionare **fatture**
- Fare clic su **Scarica fattura** per visualizzare una copia della fattura PDF. Se si dice che **non è disponibile** , vedere [perché non viene visualizzata una fattura per l'ultimo periodo di fatturazione?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

**Ricevere la fattura tramite posta elettronica (. pdf)**

- Selezionare l'abbonamento dalla pagina [abbonamenti](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) . Fare clic su **fatture** e quindi inviare la fattura tramite posta elettronica
- Fare clic su **opt-in** e accettare i termini. Sarà necessario optare per ogni sottoscrizione di propria iniziativa

Nota: se non si riceve un messaggio di posta elettronica dopo aver eseguito la procedura, verificare che l'indirizzo di posta elettronica sia corretto nelle [Preferenze di comunicazione del profilo](https://account.windowsazure.com/profile) .

**Scaricare i dati di utilizzo dal portale di Azure**

- Accedere al [centro account di Azure](https://account.windowsazure.com/Subscriptions) come [amministratore dell'account](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- Selezionare l'abbonamento per cui si desidera visualizzare le informazioni sulla fattura e sull'utilizzo
- Selezionare **Cronologia fatturazione**
- Selezionare **Visualizza istruzione corrente** per visualizzare una stima dei costi nel momento in cui è stata generata la stima
- Selezionare **Scarica utilizzo** per scaricare i dati di utilizzo giornalieri come file CSV. Se sono disponibili due versioni, scaricare la versione 2

Per altre domande: [consultare i documenti sulle istanze riservate](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Documenti consigliati**

- [Nozioni di base sulla fatturazione](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Informazioni sul modo in cui viene applicato lo sconto per l'istanza riservata](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Scaricare o visualizzare la fattura di fatturazione di Azure e i dati di utilizzo giornalieri](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Informazioni sul modo in cui viene applicato lo sconto per l'istanza riservata](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Informazioni sull'utilizzo di istanze riservate per l'abbonamento pay-as-you-go](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Informazioni sull'utilizzo di istanze riservate per la registrazione dell'organizzazione](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Costi software Windows non inclusi nelle istanze riservate](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Istanze riservate nel programma del provider di soluzioni del cloud centrale (CSP) partner](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)