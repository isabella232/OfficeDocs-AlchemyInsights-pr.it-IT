---
title: Errori di creazione di eventi live in Yammer
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
- "9002495"
- "5112"
ms.openlocfilehash: 383943d670c935403fb7f4466a72474120e27e7a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825519"
---
# <a name="live-events-in-yammer-creation-errors"></a>Errori di creazione di eventi live in Yammer

**Creazione di eventi live in Yammer**

Yammer mostra sempre l'opzione per creare un evento live. In alcuni casi, è possibile che un utente non soddisfi i prerequisiti per la creazione di un evento live e che venga visualizzato un messaggio di errore quando tenta di crearlo. Di seguito sono indicate le cause più comuni di questo problema e sono illustrati alcuni modi per risolverlo per gli utenti finali.

**Chi può creare eventi live**
- Una licenza di Office 365 Enterprise E1, E3 o E5 o una licenza di Office 365 A3 o A5.
- Autorizzazioni per la creazione di eventi live nell'interfaccia di amministrazione di Microsoft Teams.
- Autorizzazioni per la creazione di eventi live in Microsoft Stream (per gli eventi prodotti con un'app o un dispositivo di trasmissione esterno).
- Appartenenza completa a un team dell'organizzazione (non si può essere guest o di un'altra organizzazione).
- Pianificazione di riunioni private, condivisione dello schermo e condivisione di video IP attivate nei criteri per le riunioni del team.

**Criteri di creazione di eventi live**

Yammer segue i criteri per gli eventi live impostati nel tenant di Office 365 per Stream. Per impostazione predefinita, tutti gli utenti dell'organizzazione possono creare un evento live. Gli amministratori potrebbero [apportare modifiche a questa impostazione che potrebbero impedire agli utenti di creare un evento live](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating). È importante verificare che gli utenti dispongano delle autorizzazioni per creare eventi live se ricevono un errore relativo ai criteri.
