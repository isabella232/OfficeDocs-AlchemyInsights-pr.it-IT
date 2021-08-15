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
ms.openlocfilehash: 7377f77b7295e8134673c9a46fa7606842d4df949f535878d13986c6d39d0b5e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53993897"
---
# <a name="delete-tenant"></a>Elimina tenant

Per eliminare azure AD, verificare:
- L'utente è un amministratore globale della directory.
- NON è stato eseguito l'accesso con un account con la directory predefinita, ad esempio contoso.onmicrosoft.com nell'account connesso, ad esempio admin@contoso.onmicrosoft.com.
- Rimuovere tutte le applicazioni attive nella directory prima dell'eliminazione. Per rimuovere le applicazioni attive, passare a Registrazioni app e rimuovere le applicazioni esistenti.
- Non sono disponibili sottoscrizioni attive per Microsoft Online Services, ad esempio Microsoft Azure, Office 365 o Azure AD Premium nella directory. Trasferire le sottoscrizioni o accelerare l'annullamento delle sottoscrizioni attive tramite il supporto e la fatturazione di Azure. Per altre informazioni, vedere Come annullare Office 365 e sottoscrizioni di Azure. Per indicazioni sull'associazione o sull'aggiunta di una sottoscrizione esistente a un tenant, vedere Associare o aggiungere una sottoscrizione [di Azure al tenant di Azure AD.](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory)
- Nessuna licenza attiva. Per rimuovere licenze, vedere [Come rimuovere la sottoscrizione per rimuovere la licenza.](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription)
- Non ci sono altri utenti attivi nella directory oltre a te come amministratore globale quando tenti di eliminare Azure AD. Rimuovere eventuali altri utenti attivi e sarà necessario rimuovere anche eventuali dipendenze da un nome di dominio personalizzato nel tenant, ad esempio gli utenti creati con admin@contoso.com.

Per ulteriori informazioni su come:
- Eliminare "Azure Active Directory" o "sottoscrizione", vedere [Delete Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).
- Rimozione di applicazioni nella directory, vedere [Rimozione di applicazioni](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app). 
