---
title: Provisioning degli utenti
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
- "9004348"
- "8428"
ms.openlocfilehash: 12490df735ca8c524058404df92db79c6c5682fe2ecafe2b42baed70fa3ab142
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971343"
---
# <a name="user-provisioning"></a>Provisioning degli utenti

- Usa la [funzionalità di provisioning su](https://docs.microsoft.com/azure/active-directory/app-provisioning/provision-on-demand) richiesta per eseguire il provisioning di un utente e ottenere una diagnostica dettagliata sui passaggi evasi.
- Per risolvere i problemi che vengono riscontrati durante il provisioning di utenti e gruppi, vedere la guida alla risoluzione dei problemi [Non è stato eseguito il provisioning di alcun utente](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-config-problem-no-users-provisioned).
- Qualora non venisse eseguito il provisioning di alcun utente, vedere [Registri del provisioning (anteprima)](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs) in Azure Active Directory (AD). Cercare voci di registro appartenenti a un utente specifico.
- Riavviare periodicamente il provisioning per rilevare eventuali utenti persi in un ciclo di provisioning precedente.
- Il provisioning dell'utente/gruppo potrebbe non essere stato eseguito perché il servizio non ha ancora avuto la possibilità di valutare l'utente. Esaminare le indicazioni per il tempo necessario per il provisioning e l'indicatore di stato nella pagina di configurazione del provisioning. Se lo stato costante specificato nella sezione dettagli aggiuntivi è precedente alla data in cui l'utente è stato creato/aggiornato/eliminato, significa che l'utente non è stato ancora valutato. In questo scenario, la cosa migliore da fare è attendere il completamento del servizio di provisioning. Se lo stato stabile è stato raggiunto, ti consigliamo di eseguire un riavvio dall'interfaccia utente nel portale di Azure.
  - Tenere presente che il servizio è a conoscenza solo delle modifiche apportate a un utente/gruppo nel sistema di origine (Azure Active Directory). Se un utente/gruppo viene rimosso direttamente nell'applicazione (ad esempio, ServiceNow), non si è a conoscenza di tali modifiche e non ne viene eseguito il rollback in base allo stato dell'utente nel sistema di origine. In questo scenario, è meglio eseguire il rollback della modifica direttamente nell'applicazione di destinazione.
- Il servizio ha valutato l'utente/gruppo e ha determinato che non deve essere eseguito il provisioning:
  - Se l'ambito è stato impostato su utenti e gruppi assegnati, verificare se l'utente/gruppo è assegnato all'applicazione.
  - Se l'utente/gruppo è assegnato all'applicazione, assicurarsi che non sia assegnato al ruolo di accesso predefinito. Questo ruolo non può essere usato per il provisioning.
  - Se è stato impostato un filtro di ambito basato su attributo, verificare che l'utente soddisfi i criteri specificati.
  - Se gli utenti sono già presenti nel sistema di destinazione e lo stato dell'utente nella corrispondenza di origine e destinazione, non verrà eseguita alcuna ulteriore azione.
- Il servizio ha tentato di eseguire il provisioning dell'utente e non è riuscito. Per questi scenari, esaminare la scheda risoluzione dei problemi e suggerimenti dei log di provisioning:
  - Un attributo obbligatorio dell'utente potrebbe non essere presente Azure Active Directory o non corrisponde al formato richiesto dall'applicazione di terze parti. Ad esempio, l'attributo Country per un utente potrebbe essere impostato su Stati Uniti quando dovrebbe essere US.
  - L'attributo è un attributo referenziale che non esiste ancora nell'applicazione di destinazione. Un attributo referenziale è un attributo che punta a un altro oggetto, ad esempio un utente membro di un gruppo. L'ID dell'utente si trova nell'attributo member del gruppo, ma può essere elaborato solo se l'oggetto utente a cui punta esiste già.
