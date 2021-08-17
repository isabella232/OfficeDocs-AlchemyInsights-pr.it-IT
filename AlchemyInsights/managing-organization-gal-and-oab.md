---
title: Gestione dell'elenco indirizzi globale e della rubrica offline dell'organizzazione
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
- "9002895"
- "5550"
ms.openlocfilehash: c5b73e2dae4d2b98b6af05e147f93a493bac5a88cfcb9ea67c979264aba34ceb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54042166"
---
# <a name="managing-organization-global-address-list-gal-and-offline-address-book-oab"></a>Gestione dell'elenco indirizzi globale e della rubrica offline dell'organizzazione

Un elenco indirizzi globale è un elenco di oggetti abilitati per la posta elettronica, ossia qualunque tipo di destinatario che può ricevere un messaggio di posta elettronica, all'interno dell'organizzazione. In ogni organizzazione viene creato automaticamente un elenco indirizzi globale. È possibile creare altri elenchi indirizzi globali per separare gli utenti in base all'organizzazione o al luogo, ma ogni utente può visualizzare e usare un solo elenco indirizzi globale per volta.

Alcuni client di posta elettronica, come Outlook per Windows, scaricano l'elenco indirizzi globale per l'uso offline. Questo elenco è denominato rubrica offline. In Exchange Online, una rubrica offline viene aggiornata ogni 8 ore, quindi i client devono scaricarla per aggiornare la copia offline locale. Qualsiasi modifica ai destinatari deve essere visibile nell'elenco indirizzi globale prima di passare alla rubrica offline.

Di seguito sono riportate alcune procedure comuni per l'elenco indirizzi globale e la rubrica offline:

- Per vari motivi, può essere preferibile che alcuni oggetti siano nascosti dall'elenco indirizzi globale. Per ulteriori informazioni, vedere [Nascondere i destinatari dagli elenchi di indirizzi](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).
- Se è necessario assegnare visualizzazioni personalizzate dell'elenco indirizzi globale dell'organizzazione a specifici gruppi di utenti, vedere [Criteri della rubrica in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).
- [Creare un elenco indirizzi globale in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) e vedere [Elenchi di indirizzi in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists) per informazioni sull'uso delle autorizzazioni dell'elenco indirizzo globale. Tenere presente che, se si crea un nuovo elenco indirizzi globale, può essere utile creare anche una nuova rubrica offline. Vedere [Procedure relative alle rubriche offline](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).
