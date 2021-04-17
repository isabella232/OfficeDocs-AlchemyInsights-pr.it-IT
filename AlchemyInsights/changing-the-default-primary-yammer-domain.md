---
title: Modifica del dominio di Yammer predefinito
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
- "9002662"
- "5162"
ms.openlocfilehash: 6a7215ef7187e8dc6c834470b4724692b239efd4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817985"
---
# <a name="changing-the-defaultprimary-yammer-domain"></a>Modifica del dominio predefinito/primario di Yammer

L'URL di Yammer contiene il nome di dominio primario corrente per la rete Yammer. Questo nome di dominio potrebbe non corrispondere al nome di dominio primario impostato in Office 365 o Azure AD. Esistono differenze di comportamento in base al numero di domini personalizzati aggiunti al tenant e al fatto che Yammer sia o meno in una configurazione supportata (1 tenant per 1 rete o 1:1). È disponibile documentazione sui [Domini di Yammer e Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/manage-yammer-domains).

Il motivo più comune per cui viene visualizzato un dominio non corretto è che esistono più reti Yammer che devono essere consolidate. [Il consolidamento a un'unica rete](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) con lo strumento di migrazione di rete è un importante primo passaggio. Completare questa operazione prima di provare a configurare il dominio primario.

**Nessun dominio personalizzato**

Per i nuovi tenant, per Yammer verrà usato il dominio predefinito del tenant (ad esempio fabrikam.onmicrosoft.com). Il dominio primario è impostato su yammer.com/fabrikam.onmicrosoft.com.

**Singolo dominio personalizzato**

Yammer selezionerà automaticamente il dominio personalizzato del tenant, ad esempio fabrikam.com, come dominio primario in Yammer. È impostato su yammer.com/fabrikam.com. Questa modifica viene apportata dal servizio di sincronizzazione dei domini e può richiedere fino a 24 ore.

**Più domini personalizzati**

Yammer può avere un dominio primario diverso dal dominio predefinito del tenant. Poiché esistono più domini personalizzati, Yammer non cerca di indovinare il dominio corretto tra quelli disponibili. È necessario aprire un caso di supporto per richiedere che il nome di dominio primario sia modificato nel dominio primario di propria scelta.

**Ulteriori informazioni per la risoluzione dei problemi**

In alcuni casi i domini possono essere stati spostati tra tenant e il servizio di sincronizzazione dei domini non ha funzionato correttamente. È possibile che si verifichino problemi di accesso o di altro tipo, oltre alla visualizzazione del dominio primario errato. Per risolvere il problema, potrebbe essere necessario spostare i domini nella rete corretta con l'aiuto del Supporto tecnico Microsoft. Per questa situazione occorre l'assistenza diretta e la risoluzione può richiedere del tempo, soprattutto se l'elenco di nomi di dominio è molto lungo. Aprire un caso di supporto per ottenere assistenza per la risoluzione dei problemi di questo tipo.

L'agente di supporto si accerterà che i domini siano verificati in un tenant sotto il controllo dell'utente. Potrà porre ulteriori domande di verifica sui propri domini se sono aggiunti al tenant, ma non verificati tramite DNS. Assicurarsi che i domini siano verificati tramite DNS per velocizzare il processo.
