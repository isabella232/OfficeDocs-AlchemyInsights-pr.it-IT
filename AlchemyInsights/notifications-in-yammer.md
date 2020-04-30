---
title: Notifiche in Yammer
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002878"
- "5480"
ms.openlocfilehash: ff4c13560b9cbf283e5c6b92a259debdf96cca62
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/27/2020
ms.locfileid: "43911907"
---
# <a name="notifications-in-yammer"></a>Notifiche in Yammer

Per avvisarti riguardo a nuove attività nelle conversazioni pertinenti, [Yammer invia notifiche](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996) tramite posta elettronica oppure, se lo usi nel tuo dispositivo mobile, notifiche push. Per impostazione predefinita, Yammer invia notifiche per diversi tipi di attività in rete. Gli utenti possono aggiornare le impostazioni della posta elettronica dal sito Web di Yammer, mentre le notifiche push sono configurate dall'app per dispositivi mobili. 

Yammer ha aggiunto il supporto per le [e-mail interattive in Outlook](https://techcommunity.microsoft.com/t5/outlook-blog/interactive-yammer-emails-in-outlook-on-the-web-are-here/ba-p/1209420). Alcuni messaggi di posta elettronica (copia del messaggio) diventeranno interattivi all'interno di Outlook sul Web. Un aggiornamento futuro consentirà di eseguire questa operazione in altre versioni di Outlook.

**Tipi di notifiche in Yammer**

- Messaggi di posta elettronica (aggiornamenti di un gruppo, qualcuno ti invita in un gruppo, ricevi un messaggio nella posta in arrivo e così via).
- Notifiche push (inviate ai dispositivi mobili quando sei menzionato, ricevi un messaggio nella posta in arrivo e così via)
- Popup desktop (quando l'app desktop Yammer è installata, gli utenti visualizzeranno notifiche di tipo avviso popup).
- Notifiche con campanello (all'interno del sito Web di Yammer, gli utenti vedranno le notifiche per diversi eventi. Queste notifiche potrebbero non essere sempre associate a un messaggio di posta elettronica o una notifica push).

Sono disponibili altre [informazioni dettagliate sulle notifiche](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996).

**Gestione delle notifiche**

Gli utenti devono gestire le proprie notifiche. Consulta le informazioni su [come abilitare e disabilitare le notifiche di posta elettronica e per dispositivi mobili di Yammer](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996). 

Gli amministratori non possono disabilitare tutte le notifiche o controllare le notifiche per conto degli utenti. Gli amministratori possono [controllare il logo incluso nei messaggi di posta elettronica e se gli utenti devono confermare i messaggi](https://docs.microsoft.com/yammer/configure-your-yammer-network/configure-email-and-yammer) inviati tramite posta elettronica.

**Notifiche tramite posta elettronica inviate a molti utenti nell'organizzazione**

A volte una singola notifica tramite posta elettronica viene inviata da Yammer e ricevuta da molti più utenti nell'organizzazione di quanto previsto. Questo problema si verifica quando una lista di distribuzione o un altro tipo di indirizzo di posta elettronica non singolo viene aggiunto a Yammer. Yammer non rileva sempre se un indirizzo di posta elettronica appartiene a un singolo utente o se può comportare l'invio di un messaggio di posta elettronica a molti destinatari. Se si verifica questo problema, è necessario intervenire per [sospendere (disattivare) l'utente non valido con tale indirizzo di posta elettronica](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users) in Yammer. 

Per ridurre la probabilità del verificarsi di questo problema, è consigliabile:

1. [Applicare l'identità di Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity) per Yammer.
2. Impedisci ai mittenti esterni di inviare messaggi di posta elettronica all'organizzazione o limitali a un elenco approvato.

Se si verifica questo problema:

1. Identifica il destinatario del messaggio di posta elettronica, che deve corrispondere all'utente in Yammer. Ad esempio, all-in-sales@fabrikam.com è una lista di distribuzione per tutti gli addetti alle vendite. Questa lista di distribuzione sarebbe identificabile dai messaggi di posta elettronica di Yammer ricevuti dagli utenti.
2. Usa la funzionalità [disattiva (sospendi) in Amministratore di rete](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users) per sospendere l'utente con l'indirizzo di posta elettronica all-in-sales@fabrikam.com. La sospensione può essere annullata, quindi è più sicura dell'eliminazione. L'eliminazione dell'utente avverrà automaticamente dopo 90 giorni.
3. Se vuoi, puoi esaminare [Esportazione degli utenti](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data#ExportUsers) per identificare altri indirizzi di posta elettronica non utenti che devono essere sospesi.
