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
ms.openlocfilehash: e9a1e74b321e2c2dda5f7a4f69681a0acf0635d5
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 11/03/2020
ms.locfileid: "48840608"
---
# <a name="transfer-azure-billing-ownership"></a>Trasferire la proprietà della fatturazione di Azure

Accede al [portale di Azure](https://portal.azure.com/) con il ruolo di Amministratore dell'account di fatturazione che include la sottoscrizione che si vuole trasferire. Se non si è certi di essere amministratori o se è necessario determinare l'amministratore, vedere [Determinare l'amministratore della fatturazione dell'account](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).

- Cercare in **Gestione costi e fatturazione**.
- Selezionare **Sottoscrizioni** nel riquadro sinistro. A seconda del tipo di accesso, potrebbe essere necessario selezionare un ambito di fatturazione, poi **Sottoscrizioni** o **Sottoscrizioni di Azure**.
- Selezionare **Trasferisci la proprietà della fatturazione** per la sottoscrizione che si vuole trasferire
- Immettere l'indirizzo di posta elettronica dell'utente, già amministratore fatturazione dell'account, che diventerà il nuovo proprietario della sottoscrizione, poi selezionare **Invia richiesta di trasferimento**
- L'utente riceverà un messaggio di posta elettronica con le istruzioni per verificare la richiesta di trasferimento. Per approvare la richiesta, l'utente deve selezionare il collegamento nel messaggio di posta elettronica e seguire le istruzioni.

**Nota** : se si trasferisce la proprietà della fatturazione relativa alla sottoscrizione a un account utente di un altro tenant di Azure AD, tutte le assegnazioni di [Controllo accessi in base al ruolo (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) per la gestione delle risorse nella sottoscrizione verranno rimosse definitivamente. Solo il nuovo proprietario avrà accesso alla gestione delle risorse nella sottoscrizione. Per altre informazioni, vedere [Trasferimento di una sottoscrizione a un utente di un altro tenant di Azure AD](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**Documenti consigliati**

- [Trasferire la proprietà della fatturazione di una sottoscrizione di Azure a un altro account](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [Informazioni sul trasferimento della proprietà di fatturazione per una sottoscrizione di Azure](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [Trasferimento delle sottoscrizioni di Visual Studio, Microsoft Partner Network (MPN) e Sviluppo/test con pagamento in base al consumo](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Domande frequenti sul trasferimento della proprietà](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Risoluzione dei problemi relativi al trasferimento della proprietà](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
