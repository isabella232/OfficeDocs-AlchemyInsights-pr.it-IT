---
title: Perché il pulsante Aggiungi budget è disabilitato per l'utente?
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
- "9003547"
- "6464"
ms.openlocfilehash: 18edad73f617ba180cb08576ee6e5fa8faf07128
ms.sourcegitcommit: 9a7b85eae0bb775bc2498a83d8f5fedb72a6451e
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 10/27/2020
ms.locfileid: "48769590"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>Perché il pulsante Aggiungi budget è disabilitato per l'utente?

Per creare un budget, è necessario disporre di una delle autorizzazioni seguenti:

- Gruppo di gestione, sottoscrizione, ambiti di gruppi di risorse
- Collaboratore per la gestione dei costi
- Proprietario
- Collaboratore
- Solo cliente aziendale: registrazione, reparto, ambiti degli account
- Amministratore di registrazione (impostare il budget nell'ambito di registrazione)
- Amministratore del reparto (impostare il budget nell'ambito del reparto)
- Proprietario dell'account (impostare il budget nell'ambito dell'account)
- Solo contratto clienti moderno: account di fatturazione, profilo di fatturazione, ambiti sezione fattura
- Creatore della sottoscrizione di Azure

**Ho creato un budget quando il costo per il mese corrente era già troppo preventivo. Perché non si riceve un avviso?**  
Se si è già superato un determinato limite di costi quando si crea un budget che l'avviso non verrà attivato. Una volta che inizia un nuovo ciclo, se si viola la soglia, l'avviso verrà attivato.

**Quando si desidera ricevere un avviso dopo aver superato una delle soglie di avviso definite per il budget?**  
I budget vengono valutati ogni 4 ore. Per ottenere i dati di utilizzo per il sistema dei budget, è necessario un minimo di 8 ore. Dato questo, gli avvisi possono richiedere fino a 12 ore dopo aver superato una soglia.

**Perché il pulsante Data di inizio è disabilitato quando si seleziona il mese o il periodo di reimpostazione del mese di fatturazione?**  
I budget sono allineati al mese di calendario corrente o al periodo di fatturazione corrente, nel caso in cui sia selezionato il mese di fatturazione. Di conseguenza, il valore viene prepopolato per l'utente.

**Perché non viene visualizzato un grafico dei costi nell'esperienza di creazione del budget?**  
È necessario un minimo di 2 mesi di dati di costo prima di poter eseguire il rendering di un grafico per facilitare la creazione del budget.

**Perché non è possibile impostare un budget per un abbonamento appena creato?**  
Dopo la creazione di un abbonamento, i dati devono essere elaborati per 24-48 ore prima di impostare un preventivo su di esso.

**Risorse dell'API di budget**

- [Budgets API V1](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support): fornisce operazioni per la creazione e l'aggiornamento di budget. Utilizzando l'API budgets, è possibile impostare una soglia di budget e configurare più avvisi in modo che vengano attivati quando si accede a tale soglia. Gli avvisi possono attivare un messaggio di posta elettronica o un gruppo di azione di Azure per eseguire l'automazione. Nota: il filtro per l'API non è allineato al filtro/dimensioni API di query.
- [Probudgets API v2](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json): creare budget con funzionalità di filtraggio dei costi maggiori rispetto alla V1. Il filtro Allinea al contratto utilizzato nelle API di query e dimensioni. Si tratta dell'API per i budget consigliata per l'utilizzo di Moving Forward.
- [Dimensions](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support): fornisce operazioni per ottenere dimensioni supportate per l'utilizzo in una vasta gamma di ambiti. Utilizzando l'API Dimensions, è possibile recuperare un elenco di dimensioni che possono essere utilizzate come input per la generazione di query con l'API di query.
- [Query](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support): fornisce operazioni per ottenere i dati di utilizzo e costo aggregati in base alla query fornita. Utilizzando l'API di query, è possibile specificare il filtro, l'ordinamento e il raggruppamento desiderati per tutte le dimensioni disponibili (a cui si accede dall'API Dimensions).

**Costi previsti**

**Perché non vengono visualizzate le previsioni per i costi per l'analisi dei costi?**  
Per l'analisi dei costi, alcuni dei motivi per cui potrebbe mancare la proiezione di previsione sono diversi:

1. Se i dati relativi ai costi sono inferiori a 10 giorni, il grafico previsione non verrà caricato. Il modello richiede almeno 10 giorni di dati di costo recenti per proiezioni accurate
2. Se sono state selezionate date storiche, il grafico previsione non sarà visibile. Selezionare un intervallo di date con le date future per il grafico previsione da visualizzare
3. Se il tuo account ha più valute, il grafico previsto consentirà solo i costi del progetto per "tutti i costi in USD"

**Perché non viene modificata la previsione quando si apportano modifiche alle risorse personali?**  
Il modello di previsione richiede un paio di giorni per tenere conto delle modifiche apportate all'account e non rende immediate le proiezioni in base alla modifica delle risorse  
Per i passaggi maggiori di aumento o diminuzione delle risorse, il modello richiederà un tempo leggermente più lungo per adattarsi a queste modifiche in modo da tenere conto delle anomalie

**Perché la previsione aumenta dopo aver effettuato una prenotazione o un acquisto sul mercato?**  
Il modello di previsione considera il ' costo effettivo ' e non tiene conto dell'utilizzo e dell'acquisto separatamente. Per un acquisto di una tantum, il modello diminuirà le proiezioni dopo 10 giorni per rendere conto dell'improvviso aumento dei costi.

**Voglio vedere le previsioni per una singola dimensione (es. Indicatore**  
La previsione attualmente supporta le proiezioni dei costi totali e non i singoli contatori. Pertanto, quando ' raggruppato per ' una dimensione, le proiezioni saranno per il totale di tutti gli elementi nella dimensione

**Documenti consigliati**

- [Che cos'è Azure Cost Management?](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Procedure consigliate per la gestione dei costi di Azure](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Analisi dei costi e della spesa](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Esplorare e analizzare i costi con l'analisi dei costi](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Gestione dei costi di Azure: prezzi](https://azure.microsoft.com/services/cost-management/#pricing)
- [Esaminare i costi nell'analisi dei costi](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [Video tutorial: creare un budget nel portale di Azure](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [Prerequisiti per la visualizzazione e la personalizzazione dei budget](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [Creare e gestire i budget](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [Configurare l'automazione con i gruppi di azione di Azure e i budget API](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [Utilizzare gli avvisi sui costi per monitorare l'utilizzo e la spesa](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Procedure consigliate per la gestione dei costi](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**Video sull'esercitazione**

- [Creare un budget nel portale di Azure](https://go.microsoft.com/fwlink/?linkid=2146761)
- [Gestire i costi con l'API per i budget e i gruppi di azione](https://go.microsoft.com/fwlink/?linkid=2147038)