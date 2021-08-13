---
title: Perché il pulsante Aggiungi budget è disabilitato?
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
- "9003547"
- "6464"
ms.openlocfilehash: 1263662184948ed1e77e3abacd17babf4aa033ed1ecec29b4c4afc26d6da56f0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53954675"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>Perché il pulsante Aggiungi budget è disabilitato?

Per creare un budget, è necessaria una delle autorizzazioni seguenti:

- Gruppi di gestione, sottoscrizione, ambiti di gruppi di risorse
- Collaboratore gestione costi
- Proprietario
- Collaboratore
- Enterprise Solo cliente: registrazione, reparto, ambiti account
- Amministratore registrazione (impostare il budget nell'ambito di registrazione)
- Amministratore reparto (impostare il budget nell'ambito del reparto)
- Proprietario dell'account (impostare il budget nell'ambito dell'account)
- Solo contratto cliente moderno: account di fatturazione, profilo di fatturazione, ambiti della sezione fattura
- Creatore della sottoscrizione di Azure

**È stato creato un budget quando il costo per il mese corrente era già troppo elevato. Perché non ho ricevuto un avviso?**  
Se hai già superato una determinata soglia di costo quando crei un budget che non genera l'avviso. Una volta avviato un nuovo ciclo, se si supera la soglia, l'avviso verrà generato.

**Quando devo aspettarmi di ricevere un avviso dopo aver superato una delle soglie di avviso del budget definite?**  
I budget vengono valutati ogni 4 ore. Sono necessari almeno 8 ore prima che i dati di utilizzo raggiungano il sistema di budget. In questo caso, gli avvisi possono richiedere fino a 12 ore dopo il superamento di una soglia.

**Perché il pulsante Data inizio è disabilitato quando si seleziona un periodo di reimpostazione mese o fatturazione?**  
I budget sono allineati al mese di calendario corrente o al periodo di fatturazione corrente (nel caso in cui sia selezionato Mese fatturazione). Pertanto, precompimo questo valore automaticamente.

**Perché non viene visualizzato un grafico dei costi nell'esperienza di creazione del budget?**  
Abbiamo bisogno di almeno 2 mesi di dati sui costi prima di poter eseguire il rendering di un grafico per agevolare la creazione del budget.

**Perché non è possibile impostare un budget per una sottoscrizione appena creata?**  
Dopo la creazione di una sottoscrizione, l'elaborazione dei dati richiede 24-48 ore prima di impostare un budget.

**Risorse API preventivo**

- [API budget v1](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support): fornisce le operazioni per creare e aggiornare i budget. Usando l'API Budgets, puoi impostare una soglia di budget e configurare più avvisi in modo che si attivino quando ti avvicini a tale soglia. Gli avvisi possono attivare un messaggio di posta elettronica o un gruppo di azioni di Azure per eseguire l'automazione. Nota: il filtro per questa API non è allineato al filtro/dimensioni dell'API di query.
- [API budget v2](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json): creare budget con funzionalità di filtro dei costi maggiori rispetto alla v1. Il filtro è allineato al contratto usato nelle API Query e Dimensioni. Questa è l'API di budget consigliata per l'uso in futuro.
- [Dimensioni](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support): fornisce operazioni per ottenere le dimensioni supportate per l'utilizzo in un'ampia gamma di ambiti. Usando l'API Dimensions, puoi recuperare un elenco di dimensioni che possono essere usate come input per generare query con l'API query.
- [Query](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support): fornisce operazioni per ottenere dati aggregati sui costi e sull'utilizzo in base alla query fornita. Usando l'API query, puoi specificare il filtro, l'ordinamento e il raggruppamento desiderati in tutte le dimensioni disponibili (a cui è possibile accedere dall'API Dimensions).

**Costi previsti**

**Perché non vengono visualizzati i costi previsti nell'analisi dei costi?**  
Esistono diversi motivi per cui la proiezione di previsione potrebbe non essere presente nell'analisi dei costi, alcuni dei quali sono i seguenti:

1. Se i dati relativi ai costi hanno meno di 10 giorni, il grafico delle previsioni non verrà caricato. Il modello richiede almeno 10 giorni di dati sui costi recenti per proiezioni accurate
2. Se sono state selezionate date storiche, il grafico delle previsioni non sarà visibile. Selezionare un intervallo di date con date future per il grafico delle previsioni da visualizzare
3. Se l'account ha più valute, il grafico delle previsioni includerà solo i costi di progetto per "Tutti i costi in USD"

**Perché la previsione non cambia quando si apportano modifiche alle risorse?**  
Il modello previsionale richiede un paio di giorni per prendere in considerazione le modifiche dell'account e non effettua proiezioni immediate basate sul cambiamento delle risorse  
Per passaggi più grandi di aumento o riduzione delle risorse, il modello richiederà un po' di più per adattarsi a queste modifiche per prendere in considerazione le anomalie

**Perché le previsioni aumentano dopo aver fatto una prenotazione o un acquisto marketplace?**  
Il modello previsionale considera il "Costo effettivo" e non considera l'utilizzo e l'acquisto separatamente. Per un acquisto una sola volta, il modello ridurrà le proiezioni dopo 10 giorni per conto dell'improvviso aumento dei costi

**Si desidera visualizzare le previsioni per una singola dimensione (ad esempio. Meter)**  
La previsione attualmente supporta proiezioni di costo totale e non per singoli metri. Di conseguenza, quando viene "raggruppato per" una dimensione, le proiezioni saranno per il totale di tutti gli elementi nella dimensione

**Documenti consigliati**

- [Che cos'è Azure Cost Management?](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Procedure consigliate per la gestione dei costi di Azure](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Analizzare i costi e le spese](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Esplorare e analizzare i costi con l'analisi dei costi](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Gestione dei costi di Azure: prezzi](https://azure.microsoft.com/services/cost-management/#pricing)
- [Esaminare i costi nell'analisi dei costi](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [Esercitazione video: Creare un budget nel portale di Azure](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [Prerequisiti per la visualizzazione e la personalizzazione dei budget](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [Creare e gestire budget](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [Configurare l'automazione con i gruppi di azioni di Azure e l'API budget](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [Usare gli avvisi costi per monitorare l'utilizzo e la spesa](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Procedure consigliate per la gestione dei costi](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**Video sulle esercitazioni**

- [Creare un budget nel portale di Azure](https://go.microsoft.com/fwlink/?linkid=2146761)
- [Gestire i costi con l'API Budgets e i gruppi di azioni](https://go.microsoft.com/fwlink/?linkid=2147038)