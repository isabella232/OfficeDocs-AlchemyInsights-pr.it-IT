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
ms.openlocfilehash: 8d8821cda94b2af244fa317707421f9d197b6052fb316789cd286ea8b4adf19e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960155"
---
# <a name="problem-with-single-user"></a>Problema con un singolo utente

- Il provisioning dell'utente potrebbe non essere stato eseguito perché il servizio non ha ancora avuto la possibilità di valutare l'utente. Esaminare le indicazioni per il tempo necessario per il provisioning e l'indicatore di stato nella pagina di configurazione del provisioning. Se lo stato costante specificato nella sezione dettagli aggiuntivi è precedente alla data in cui l'utente è stato creato/aggiornato/eliminato, significa che l'utente non è stato ancora valutato. In questo scenario, la cosa migliore da fare è attendere il completamento del servizio di provisioning.

  - Tieni presente che il servizio è a conoscenza solo delle modifiche apportate a un utente nel sistema di origine (Cloud HR). Deve essere presente una modifica valida nel sistema di origine per Azure AD per rilevare la modifica e scorrerla in Active Directory.
- Il servizio di provisioning ha valutato l'utente e ha determinato che non deve essere eseguito il provisioning:
  - Se è stato impostato un filtro di ambito basato su attributo, verificare che l'utente soddisfi i criteri specificati.
  - Se gli utenti sono già presenti nel sistema di destinazione e lo stato dell'utente nella corrispondenza di origine e destinazione, non verrà eseguita alcuna ulteriore azione.
- Il servizio di provisioning ha tentato di eseguire il provisioning dell'utente e non è riuscito. Per questi scenari, esaminare la scheda risoluzione dei problemi e suggerimenti dei log di provisioning:
  - Un attributo obbligatorio per l'utente potrebbe non essere presente in Active Directory locale o Azure AD. Ad esempio, le regole di generazione userPrincipalName o sAMAccountName non generano il valore giusto.
  - L'attributo corrispondente (in genere employeeId) non viene risolto in un utente univoco in Active Directory locale o Azure AD. Ad esempio, ci sono due utenti con lo stesso employeeId in Active Directory e il servizio restituisce un codice di errore che indica le voci di destinazione duplicate per la stessa voce di origine.

Per esaminare i log per singoli utenti e gruppi, vedere [Review the provisioning logs for an issue with a specific user](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).
