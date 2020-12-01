---
title: Elimina tenant
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/30/2020
ms.locfileid: "49477675"
---
# <a name="delete-tenant"></a>Elimina tenant

Per eliminare un annuncio di Azure, verificare quanto segue:
- Si è un amministratore globale nella directory.
- L'utente non ha eseguito l'accesso con un account che include la directory predefinita, ad esempio contoso.onmicrosoft.com, nell'account signed-in, ad esempio admin@contoso.onmicrosoft.com.
- Rimuovere tutte le applicazioni attive nella directory prima dell'eliminazione. Per rimuovere le applicazioni attive, passare a registrazioni delle app e rimuovere le applicazioni esistenti.
- Non vi sono abbonamenti attivi per i Microsoft Online Services, ad esempio Microsoft Azure, Office 365 o Azure AD Premium associati alla directory. Trasferire gli abbonamenti o velocizzare l'annullamento di abbonamenti attivi tramite il supporto e la fatturazione di Azure. Per ulteriori informazioni, vedere Annullamento delle sottoscrizioni di Office 365 e Azure. Per informazioni sull'associazione o l'aggiunta di una sottoscrizione esistente a un tenant, vedere [associare o aggiungere una sottoscrizione di Azure al tenant di Azure ad](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).
- Non sono disponibili licenze attive. Per rimuovere le licenze, vedere [come rimuovere la sottoscrizione per rimuovere la licenza](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).
- Non ci sono altri utenti attivi nella directory oltre all'amministratore globale quando si tenta di eliminare l'Azure AD. Rimuovere qualsiasi altro utente attivo e devono essere rimosse anche eventuali dipendenze su un nome di dominio personalizzato nel tenant, ad esempio gli utenti creati con admin@contoso.com.

Per ulteriori informazioni su come eseguire le operazioni seguenti:
- Eliminare "Azure Active Directory" o "sottoscrizione", vedere [Delete Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).
- Rimozione di applicazioni nella directory, vedere [rimozione di applicazioni](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app). 
