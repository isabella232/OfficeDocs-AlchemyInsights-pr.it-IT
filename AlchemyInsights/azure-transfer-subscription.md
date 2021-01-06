---
title: Trasferire la proprietà della fatturazione di Azure
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
- "9003560"
- "6849"
ms.openlocfilehash: 74b7cc879973790b7532106c80b718856682a334
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755551"
---
# <a name="transfer-azure-billing-ownership"></a>Trasferire la proprietà della fatturazione di Azure

Accedere al [portale di Azure](https://portal.azure.com/) con il ruolo di Amministratore dell'account di fatturazione che include la sottoscrizione che si desidera trasferire. Se non si è certi di essere amministratori o se è necessario determinare chi sia l'amministratore, vedere [Determinare l'amministratore fatturazione dell'account](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).

1. Cercare _Gestione costi e fatturazione_.
1. Selezionare **Sottoscrizioni** nel riquadro sinistro. A seconda del tipo di accesso, potrebbe essere necessario selezionare un ambito di fatturazione, quindi **Sottoscrizioni** o **Sottoscrizioni di Azure**.
1. Selezionare **Trasferire la proprietà della fatturazione** per la sottoscrizione che si desidera trasferire.
1. Immettere l'indirizzo di posta elettronica di un utente che sia amministratore fatturazione dell'account, che diventerà il nuovo proprietario della sottoscrizione, quindi selezionare **Invia richiesta di trasferimento**.
1. L'utente riceverà un messaggio di posta elettronica con le istruzioni per verificare la richiesta di trasferimento. Per approvare la richiesta, è necessario che l'utente selezioni il collegamento nel messaggio di posta elettronica e segua le istruzioni.

Si noti che trasferendo la proprietà della fatturazione relativa alla sottoscrizione a un account utente di un altro tenant di Azure AD, tutte le assegnazioni del [Controllo degli accessi in base al ruolo ](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) per la gestione delle risorse nella sottoscrizione verranno rimosse definitivamente. Solo il nuovo proprietario avrà accesso alla gestione delle risorse nella sottoscrizione. Per altre informazioni su come cambiare directory per una sottoscrizione, vedere [Trasferire una sottoscrizione a un utente in un altro tenant di Azure AD](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

_**Impatto importante sulle fatture**_: se è stata la trasferita la proprietà della fatturazione per una sottoscrizione Azure, gli addebiti saranno calcolati pro-rata. Sarà possibile accedere alle fatture seguendo questa procedura:  

1. Selezionare la sottoscrizione nella  [Pagina sottoscrizioni](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) nel portale di Azure come  [utente con accesso alle fatture](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support), quindi  **Fatture**.
1. Fare clic su  **Scarica fattura**  per visualizzare una copia della fattura in formato PDF. Se è presente il messaggio  _Non disponibile_, vedere  [Perché non visualizzo la fattura per l'ultimo periodo di fatturazione?](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)
1. È possibile anche visualizzare il proprio uso giornaliero facendo clic sul **periodo di fatturazione** per ottenere un PDF della fattura e una copia del file relativo all'uso giornaliero dettagliato (.CSV). Per ulteriori informazioni, vedere [Ottenere dati su fatturazione e utilizzo](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support).

**Documenti consigliati**

- [Trasferire la proprietà della fatturazione di una sottoscrizione di Azure a un altro account](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [Informazioni sul trasferimento della proprietà di fatturazione per una sottoscrizione di Azure](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [Trasferimento delle sottoscrizioni di Visual Studio, Microsoft Partner Network (MPN) e Sviluppo/test con pagamento in base al consumo](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Domande frequenti sul trasferimento della proprietà](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Risoluzione dei problemi relativi al trasferimento della proprietà](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
