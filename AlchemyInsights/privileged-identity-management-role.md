---
title: Privileged Identity Management ruolo
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "6825"
ms.openlocfilehash: 358e446192e6b58ace81afa06e0d65ae3a207282351ffc3ec9975a24779951fb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53973233"
---
# <a name="privileged-identity-managementpim-role"></a>Privileged Identity Management(PIM)

**Le autorizzazioni non vengono concesse dopo l'attivazione di un ruolo**

Quando si attiva un ruolo in Azure AD Privileged Identity Management (PIM), l'attivazione potrebbe non propagarsi istantaneamente a tutti i portali che richiedono il ruolo con privilegi. A volte, anche se la modifica viene propagata, la memorizzazione nella cache Web in un portale potrebbe non avere effetto immediato.

Se l'attivazione è ritardata, eseguire la procedura seguente:

1. Disconnettersi dal portale di Azure e quindi accedere di nuovo. Quando attivi un ruolo di Azure AD o un ruolo di risorsa di Azure, verranno visualizzati i fasi dell'attivazione. Una volta completate tutte le fasi, verrà visualizzato un collegamento "Disconnennei". È possibile utilizzare questo collegamento per disconnettersi. Questo risolverà la maggior parte dei casi per il ritardo di attivazione.
2. In PIM, verificare di essere elencati come membri del ruolo.
3. Se si sta attivando il ruolo Exchange amministratore, assicurarsi di disconnettersi e accedere di nuovo. Se il problema persiste, aprire un ticket di supporto e genera questo problema. Se si utilizza il ruolo Exchange amministratore per accedere al Centro sicurezza e conformità, vedere il passaggio successivo.
4. Se si sta attivando un ruolo per accedere al Centro sicurezza e conformità o se si sta attivando il ruolo di amministratore di SharePoint, si verifica un ritardo di attivazione da alcuni minuti fino a poche ore. Si tratta di un problema noto e stiamo lavorando attivamente con questi team per risolvere il problema il prima possibile.

Per altre informazioni, vedere:

- [Attivare i ruoli di Azure AD in PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [Attivare i ruoli delle risorse di Azure in PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**Le autorizzazioni non vengono rimosse dopo la disattivazione di un ruolo o la scadenza dell'attivazione del ruolo**

Quando si disattiva un ruolo in Azure AD Privileged Identity Management o quando scade un periodo di attivazione dei ruoli, potrebbe verificarsi un ritardo per cui si continua ad avere accesso.

Se la disattivazione è ritardata, eseguire la procedura seguente:

1. Se si sta disattivando il ruolo di amministratore di Exchange o il periodo di attivazione del ruolo scade e si nota un ritardo significativo prima che le autorizzazioni siano rimosse, aprire un ticket di supporto e indicare al tecnico del supporto tecnico di invii un ticket al team pam (Privileged Access Management) all'interno di Office su questo problema.
2. Se il periodo di attivazione è scaduto, ma la sessione del browser è ancora aperta, chiudere il browser. È possibile continuare a utilizzare il ruolo fino alla chiusura della sessione. Si tratta di un problema noto e stiamo esaminando una potenziale correzione per revocare attivamente ogni sessione dopo la scadenza dell'attivazione.

Se il ritardo è diverso da questi due scenari, aprire un ticket di supporto.
