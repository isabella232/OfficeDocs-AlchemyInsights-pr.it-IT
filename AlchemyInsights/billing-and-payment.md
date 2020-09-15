---
title: Fatturazione e pagamento
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001669"
- "3752"
ms.openlocfilehash: e1f40da41eddc56c8086881a426bddb363c92446
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47686034"
---
# <a name="billing-and-payment"></a>Fatturazione e pagamento

Le bollette possono essere trovate nella **Billing**  >  scheda[pagamenti & pagamento](https://go.microsoft.com/fwlink/p/?linkid=848039) .  Per impostazione predefinita, vengono visualizzati gli ultimi 3 mesi di fatture.  Per visualizzare le fatture precedenti, modificare il filtro.  Fare clic sul collegamento **Scarica fattura PDF** per visualizzare la fattura.

**Ricevere fatture tramite posta elettronica**

Nella pagina **Billing**  >  [notifiche fatturazione](https://go.microsoft.com/fwlink/p/?linkid=853212) fatturazione, è possibile abilitare questa funzionalità e **on** gestire gli utenti che riceveranno la fattura come allegato di posta elettronica. La fattura verrà inviata agli indirizzi di posta elettronica degli utenti nell'elenco dei destinatari delle notifiche. L'elenco include tutti gli amministratori di fatturazione e globali.  È possibile gestire gli utenti che ricevono le notifiche delle fatture cambiando il ruolo.  La rimozione del ruolo di amministratore globale o di fatturazione consente di rimuovere l'utente dall'elenco dei destinatari e l'aggiunta del ruolo di amministratore globale o di fatturazione aggiunge l'utente all'elenco dei destinatari.

**Nota**: si riceveranno due messaggi di posta elettronica distinti: uno che consente di sapere che la bolletta è pronta, con le istruzioni per accedere all'interfaccia di amministrazione per visualizzarlo e un secondo messaggio di posta elettronica che contiene l'estratto conto come allegato.

**Pagamento**

Se si paga con carta di credito o conto corrente bancario, il metodo di pagamento associato agli abbonamenti viene addebitato entro pochi giorni dopo la creazione della fattura. Se il pagamento ha esito negativo, aggiornare o modificare il metodo di pagamento.

Se è stata aggiunta una nuova scheda e si riceve un avviso di rifiuto sulla vecchia carta di credito, potrebbe essere necessario associare la nuova scheda alla sottoscrizione.

1. Nell'interfaccia di amministrazione passare alla pagina **Fatturazione** > **Fatture e pagamenti** > [Modalità di pagamento](https://go.microsoft.com/fwlink/p/?linkid=2018806).

2. Selezionare la riga della modalità di pagamento da sostituire. Nel riquadro destro sono elencati tutti i profili di fatturazione e i singoli abbonamenti che usano la modalità di pagamento selezionata.

3. Nel riquadro destro selezionare **Sostituisci metodo di pagamento per tutti gli articoli**.

4. Per usare una modalità di pagamento esistente, sceglierne una nell'elenco a discesa, quindi selezionare **Sostituisci**.

    > [!NOTE]
    > Se si hanno abbonamenti associati a un profilo di fatturazione, si può usare solo una carta di credito o di debito per il pagamento. Se nella pagina **Modalità di pagamento** sono elencati conti bancari, non sono disponibili per la selezione nell'elenco a discesa.

5. Per aggiungere una nuova modalità di pagamento, selezionare **Aggiungi modalità di pagamento**.

6. Nel riquadro **Aggiungi un metodo di pagamento** immetti le informazioni sull'account e scegli **Salva**. È necessario usare una modalità di pagamento dello stesso paese/area geografica del tenant.

7. La nuova modalità di pagamento è già selezionata nell'elenco a discesa. Selezionare **Sostituisci**.

Per altre informazioni, vedere [Gestire i metodi di pagamento](https://docs.microsoft.com/microsoft-365/commerce/billing-and-payments/manage-payment-methods).

**Frequenza di fatturazione**

Le fatture vengono generate mensilmente o annualmente a seconda della frequenza di fatturazione scelta al momento del checkout.  

**Nota**: gli ordini con fatturazione annuale possono ricevere una bolletta intermedia se sono state apportate modifiche, ad esempio l'aggiunta o la rimozione di licenze. [Modificare la frequenza di fatturazione](https://docs.microsoft.com/microsoft-365/commerce/billing-and-payments/change-payment-frequency).
