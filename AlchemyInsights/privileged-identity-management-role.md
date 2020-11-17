---
title: Ruolo di gestione delle identità con privilegi
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
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086380"
---
# <a name="privileged-identity-managementpim-role"></a>Ruolo di gestione delle identità privilegiate (PIM)

**Le autorizzazioni non vengono concesse dopo l'attivazione di un ruolo**

Quando si attiva un ruolo in Azure AD Privileged Identity Management (PIM), l'attivazione potrebbe non essere immediatamente propagata a tutti i portali che richiedono il ruolo privilegiato. A volte, anche se la modifica viene propagata, la memorizzazione nella cache Web in un portale può comportare la modifica che non avrà effetto immediato.

Se l'attivazione è ritardata, eseguire la procedura seguente:

1. Disconnettersi dal portale di Azure e quindi eseguire di nuovo l'accesso. Quando si attiva un ruolo di Azure AD o un ruolo risorsa di Azure, vengono visualizzate le fasi dell'attivazione. Una volta completate tutte le fasi, verrà visualizzato il collegamento "Esci". È possibile utilizzare questo collegamento per disconnettersi. Questo risolverà la maggior parte dei casi per il ritardo di attivazione.
2. In PIM, verificare che sia elencato come membro del ruolo.
3. Se si sta attivando il ruolo di amministratore di Exchange, assicurarsi di disconnettersi e di accedere nuovamente. Se il problema persiste, aprire un ticket di supporto e sollevarlo come problema. Se si utilizza il ruolo di amministratore di Exchange per accedere al centro sicurezza e conformità, vedere il passaggio successivo.
4. Se si sta attivando un ruolo per accedere al centro sicurezza e conformità o se si sta attivando il ruolo di amministratore di SharePoint, si verificherà un ritardo di attivazione di alcuni minuti fino a poche ore. Si tratta di un problema noto e stiamo lavorando attivamente con questi team per risolvere il problema nel più breve tempo possibile.

Per ulteriori informazioni, vedere:

- [Attivare i ruoli di Azure AD in PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [Attivare i ruoli delle risorse di Azure in PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**Le autorizzazioni non vengono rimosse dopo la disattivazione di un ruolo o la scadenza dell'attivazione del ruolo**

Quando si disattiva un ruolo in Azure AD Privileged Identity Management o quando il periodo di attivazione di un ruolo scade, potrebbe verificarsi un ritardo in cui si continuerà a essere in grado di accedere.

Se la disattivazione è in ritardo, procedere come segue:

1. Se si disattiva il ruolo di amministratore di Exchange o il periodo di attivazione del ruolo scade e si nota un ritardo significativo prima della rimozione delle autorizzazioni, aprire un ticket di supporto e informare il tecnico del supporto per l'archiviazione di un ticket con il team di gestione degli accessi con privilegi (PAM) in Office su questo problema.
2. Se il periodo di attivazione è scaduto, ma la sessione del browser è ancora aperta, chiudere il browser. È possibile continuare a utilizzare il ruolo fino a quando non viene chiusa la sessione. Si tratta di un problema noto e si tratta di una possibile soluzione che consente di revocare attivamente ogni sessione una volta scaduta l'attivazione.

Se il ritardo è diverso rispetto a questi due scenari, aprire un ticket di supporto.
