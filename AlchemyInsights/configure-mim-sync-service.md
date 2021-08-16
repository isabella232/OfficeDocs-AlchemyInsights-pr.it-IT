---
title: Configurare il servizio MIM Sync
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8472"
- "9004688"
ms.openlocfilehash: f834bead0b6f22dcadc808d45dcefe7f6571ef62c74b7fd97355157ca49542af
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53978489"
---
# <a name="configure-mim-sync-service"></a>Configurare il servizio MIM Sync

Il servizio di sincronizzazione Microsoft Identity Manager (MIM) è un componente di MIM. Si tratta di un servizio centralizzato locale che archivia e integra le informazioni per le organizzazioni che dispongono di più directory e database locali. Potrebbe essere possibile risolvere il problema con MIM Sync qualora fosse stato risolto da un aggiornamento recente di MIM o fosse tra i problemi menzionati nella sezione che segue.

**Passaggi consigliati**

1. Assicurati di usare un aggiornamento recente di MIM Sync e controlla le [note sulla versione di MIM Sync](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) per scoprire se il problema è stato risolto in un aggiornamento.
2. Se il problema si riferisce a LDAP generico, SQL generico, Lotus Domino o a un connettore ai servizi Web, assicurati di usare un aggiornamento recente dei [connettori generici](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history).
3. Se un'esecuzione di MIM Sync si interrompe con un errore, consulta la tabella dei [codici di errore](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) per determinarne le cause potenziali.
4. Se l'esecuzione viene interrotta con **extension-dll-exception**, fai clic su queste parole per aprire la finestra delle **proprietà dell'oggetto spazio connettore** e fai clic su **Analisi dello stack...** per visualizzare altre informazioni sulla causa sottostante, come descritto in [Extension-DLL-Exception](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx).
5. Se il componente Password Change Notification Service (PCNS) riporta l'**errore 6025** nel registro eventi durante la sincronizzazione della password, consulta la guida per la risoluzione dei problemi [PCNS segnala errore 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx).
6. Se la sincronizzazione completa con l'agente di gestione del servizio FIM fosse lenta, controllare l'impostazione **espansione automatica** per TempDB, come descritto in [Risoluzione dei problemi in caso la sincronizzazione completa sia lenta o venga sospesa](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx).
7. In caso riscontrassi un errore stopped-server con failed-creation-via-web-services durante l'utilizzo dell'agente di gestione del servizio FIM, consulta [Support-Info: failed-creation-via-web-services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) per una panoramica delle cause.

