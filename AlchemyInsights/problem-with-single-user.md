---
title: Problema con un singolo utente
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8469"
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/04/2021
ms.locfileid: "50428830"
---
# <a name="problem-with-single-user"></a>Problema con un singolo utente

- Il provisioning dell'utente potrebbe non essere stato eseguito perché il servizio non ha ancora avuto la possibilità di valutare l'utente. Esaminare le indicazioni relative al tempo necessario per il provisioning e la barra di avanzamento nella pagina di configurazione del provisioning. Se lo stato stabile specificato nella sezione dei dettagli aggiuntivi è precedente alla data di creazione/aggiornamento/eliminazione dell'utente, significa che non è stato ancora valutato l'utente. In questo scenario, la cosa migliore da fare è attendere il completamento del servizio di provisioning.

  - Tieni presente che il servizio è a conoscenza solo delle modifiche apportate a un utente nel sistema di origine (Cloud HR). Deve essere presente una modifica valida nel sistema di origine in modo che Azure AD rilevi la modifica e la trasla in Active Directory.
- Il servizio di provisioning ha valutato l'utente e ha determinato che non deve essere effettuato il provisioning:
  - Se è stato impostato un filtro di ambito basato su attributi, verificare che l'utente soddisfi i criteri specificati.
  - Se gli utenti esistono già nel sistema di destinazione e lo stato dell'utente nella corrispondenza di origine e destinazione, non eseguiremo ulteriori azioni.
- Il servizio di provisioning ha tentato di eseguire il provisioning dell'utente e non è riuscito. Per questi scenari, esaminare la scheda per la risoluzione dei problemi e gli elementi consigliati dei log di provisioning:
  - Un attributo obbligatorio per l'utente potrebbe non essere presente in Active Directory locale o Azure AD. Ad esempio, le regole di generazione userPrincipalName o sAMAccountName non generano il valore giusto.
  - L'attributo corrispondente (in genere employeeId) non risolve un utente univoco in Active Directory locale o Azure AD. Ad esempio, ci sono due utenti con lo stesso employeeId in Active Directory e il servizio restituisce un codice di errore che indica voci di destinazione duplicate per la stessa voce di origine.

Per esaminare i log per singoli utenti e gruppi, vedere [Esaminare i log di provisioning per un problema con un utente specifico.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs)
