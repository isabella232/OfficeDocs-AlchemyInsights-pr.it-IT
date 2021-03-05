---
title: Provisioning dell'utente
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
ms.openlocfilehash: bd415b2d44bccf0c2b3eccb4e38452498b748b3a
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430747"
---
# <a name="user-provisioning"></a>Provisioning dell'utente

- Usa la [funzionalità di provisioning su richiesta](https://docs.microsoft.com/azure/active-directory/app-provisioning/provision-on-demand) per eseguire il provisioning di un utente e ottenere una diagnostica dettagliata sui passaggi evasi.
- Per risolvere i problemi che vengono riscontrati durante il provisioning di utenti e gruppi, vedere la guida alla risoluzione dei problemi [Non è stato eseguito il provisioning di alcun utente](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-config-problem-no-users-provisioned).
- Qualora non venisse eseguito il provisioning di alcun utente, vedere [Registri del provisioning (anteprima)](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs) in Azure Active Directory (AD). Cercare voci di registro appartenenti a un utente specifico.
- Riavviare periodicamente il provisioning per rilevare eventuali utenti persi in un ciclo di provisioning precedente.
- Il provisioning dell'utente/gruppo potrebbe non essere stato eseguito perché il servizio non ha ancora avuto la possibilità di valutare l'utente. Esaminare le indicazioni relative al tempo necessario per il provisioning e la barra di avanzamento nella pagina di configurazione del provisioning. Se lo stato stabile specificato nella sezione dei dettagli aggiuntivi è precedente alla data di creazione/aggiornamento/eliminazione dell'utente, significa che non è stato ancora valutato l'utente. In questo scenario, la cosa migliore da fare è attendere il completamento del servizio di provisioning. Se è stato raggiunto lo stato stabile, ti consigliamo di eseguire un riavvio dall'interfaccia utente nel portale di Azure.
  - Tenere presente che il servizio è a conoscenza solo delle modifiche apportate a un utente/gruppo nel sistema di origine (Azure Active Directory). Se un utente/gruppo viene rimosso direttamente nell'applicazione (ad esempio, ServiceNow), non siamo a conoscenza di tali modifiche e non ne viene eseguito il rollback in base allo stato dell'utente nel sistema di origine. In questo scenario, è meglio eseguire il rollback della modifica direttamente nell'applicazione di destinazione.
- Il servizio ha valutato l'utente/gruppo e ha stabilito che non deve essere effettuato il provisioning:
  - Se l'ambito è stato impostato su utenti e gruppi assegnati, verificare se l'utente/gruppo è assegnato all'applicazione.
  - Se l'utente/gruppo è assegnato all'applicazione, assicurarsi che non siano assegnati al ruolo di accesso predefinito. Questo ruolo non può essere utilizzato per il provisioning.
  - Se è stato impostato un filtro di ambito basato su attributi, verificare che l'utente soddisfi i criteri specificati.
  - Se gli utenti esistono già nel sistema di destinazione e lo stato dell'utente nella corrispondenza di origine e destinazione, non eseguiremo ulteriori azioni.
- Il servizio ha tentato di eseguire il provisioning dell'utente e l'operazione non è riuscita. Per questi scenari, esaminare la scheda per la risoluzione dei problemi e gli elementi consigliati dei log di provisioning:
  - Un attributo obbligatorio per l'utente potrebbe non essere presente in Azure Active Directory o non corrisponde al formato richiesto dall'applicazione di terze parti. Ad esempio, l'attributo Country per un utente potrebbe essere impostato su Stati Uniti quando dovrebbe essere US.
  - L'attributo è un attributo referenziale che non esiste ancora nell'applicazione di destinazione. Un attributo referenziale è un attributo che punta a un altro oggetto, ad esempio un utente membro di un gruppo. L'ID dell'utente si trova nell'attributo member del gruppo, ma può essere elaborato solo se l'oggetto utente a cui punta esiste già.
