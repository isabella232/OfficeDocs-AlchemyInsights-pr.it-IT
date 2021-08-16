---
title: Tipi di sottoscrizione supportati
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
- "9003560"
- "6675"
ms.openlocfilehash: f11eabdc18f708e34a6a10c67bc3e7416330cbf34aec20209b42252ffa0ab018
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072164"
---
# <a name="supported-subscription-types"></a>Tipi di sottoscrizione supportati

Verificare i tipi di sottoscrizione supportati prima di proseguire.

[Tipi di sottoscrizione supportati](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

**Trasferire la proprietà della fatturazione**

Portale di Azure quale [Amministratore dell'account](https://ms.portal.azure.com/) di fatturazione che include la sottoscrizione che si vuole trasferire

- Cercare in **Gestione costi e fatturazione**. Selezionare **Sottoscrizioni** nel riquadro sinistro. A seconda del tipo di accesso, potrebbe essere necessario selezionare un ambito di fatturazione, poi **Sottoscrizioni** o **Sottoscrizioni di Azure**.
- Selezionare Trasferisci la proprietà della fatturazione per la sottoscrizione che si vuole trasferire
- Immettere l'indirizzo di posta elettronica dell'utente, già amministratore fatturazione dell'account, che diventerà il nuovo proprietario della sottoscrizione, poi selezionare **Invia richiesta di trasferimento**
- L'utente riceverà un messaggio di posta elettronica con le istruzioni per verificare la richiesta di trasferimento. Per approvare la richiesta, è necessario che l'utente selezioni il collegamento nel messaggio di posta elettronica e segua le istruzioni.

Nota: se si trasferisce la proprietà della fatturazione della sottoscrizione a un account utente di un altro tenant di Azure AD, tutte le assegnazioni di [Controllo accessi in base al ruolo (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) per la gestione delle risorse nella sottoscrizione verranno rimosse definitivamente. Solo il nuovo proprietario avrà accesso alla gestione delle risorse nella sottoscrizione. Per altre informazioni, vedere [Trasferimento di una sottoscrizione a un utente di un altro tenant di Azure AD](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**Trasferire la proprietà della sottoscrizione**

Il trasferimento della proprietà della sottoscrizione richiede il controllo di accesso in base al ruolo (RBAC) per la gestione delle risorse della sottoscrizione che perdono l'accesso. Per altre informazioni sull'aggiunta di una sottoscrizione esistente a un tenant, vedere[ Associare o aggiungere una sottoscrizione di Azure a una Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

- Durante il trasferimento della sottoscrizione, un importo non pagato relativo al ciclo di fatturazione corrente non verrà trasferito nello strumento di pagamento nel nuovo account. L'unica informazione disponibile per gli utenti del nuovo account è il costo dell'ultimo mese di sottoscrizione. Il resto della cronologia di utilizzo e fatturazione non viene trasferito con la sottoscrizione.
- Il trasferimento della proprietà della fatturazione per le sottoscrizioni del Contratto Enterprise (EA) è supportato al momento solo nel portale del Contratto Enterprise.
- Il trasferimento di una sottoscrizione orientata al credito, ad esempio Visual Studio, BizSpark, Microsoft Partner Network, a un nuovo utente richiede una licenza di Visual Studio o Microsoft Partner Network per accettare la richiesta di trasferimento
- Tutte le risorse come macchine virtuali, dischi e siti Web, vengono trasferite correttamente nel nuovo account. Il trasferimento di sottoscrizioni tra tenant potrebbe influire sulla risorse seguenti:

**Azure AD Domain Services**

Azure Key Vault

- Potrebbero essere interessati [gli utenti e i database collegati a SQL](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support), specialmente se il cliente usa un'autenticazione correlata ad Azure Active Directory
- **I servizi delle applicazioni** configurati con l'autenticazione di Azure Active Directory potrebbero essere interessati.
- Gli account di **Visual Studio Team Services** connessi a sottoscrizioni di Azure potrebbero perdere temporaneamente l'accesso quando la sottoscrizione ad Azure viene annullata.

**Documenti consigliati**

Procedura in seguito all'accettazione della proprietà della fatturazione:

- Per mantenere la proprietà della fatturazione e modificare il tipo di sottoscrizione, fare riferimento a: [Passare la sottoscrizione di Azure a un'altra offerta](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Trasferimento delle sottoscrizioni di Visual Studio, Microsoft Partner Network (MPN) e Sviluppo/test con pagamento in base al consumo](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Trasferire la proprietà della fatturazione delle sottoscrizioni del Contratto Enterprise (EA)](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [Domande frequenti sul trasferimento della proprietà](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Risoluzione dei problemi relativi al trasferimento della proprietà](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)