---
title: Assegnare gruppi a un ruolo Azure AD
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7898"
- "9003230"
ms.openlocfilehash: feca81fe785bc45e47f6faa876230b5c7701713d
ms.sourcegitcommit: 6dc6f999e840c90694a246b90062950205679420
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 01/15/2021
ms.locfileid: "49875405"
---
# <a name="assigning-groups-to-azure-ad-role"></a>Assegnare gruppi a un ruolo Azure AD

Per assegnare a un gruppo Azure AD un'origine dell'autorità in Azure AD a un ruolo Azure AD, seguire i seguenti passaggi:

1. Creare un nuovo gruppo - Per creare un nuovo gruppo:

    a. Accedere all'interfaccia di amministrazione di Azure AD con un **ruolo di amministratore con privilegi** o con autorizzazioni di **amministratore globale**.
    b. Selezionare **Azure Active Directory > Groups > Tutti i gruppi > Nuovo gruppo**.
    c. Creare il gruppo.

2. Assegnare il ruolo al gruppo durante la creazione del gruppo o in seguito alla sua creazione.

    a. Per assegnare un ruolo al gruppo al momento della creazione del gruppo, passare ad attivare/disattivare **I ruoli Azure AD possono essere assegnati al gruppo** e creare il gruppo.
    b. Per assegnare un ruolo al gruppo in seguito alla sua creazione, passare alla scheda **Ruoli assegnati** per il gruppo appena creato e assegnare il ruolo al gruppo.  

**Gestire l'appartenenza di un gruppo a cui è stato assegnato un ruolo Azure AD**

Per impostazione predefinita, per evitare l'elevazione dei privilegi, solo gli amministratori con ruoli con privilegi e gli amministratori globali possono modificare l'appartenenza di un gruppo a cui sia stato assegnato un ruolo. Tuttavia, possono scegliere di assegnare un proprietario per tale gruppo e delegare questa attività.

Per ulteriori informazioni sull'assegnazione dei gruppi cloud ai ruoli Azure AD, vedere [Assegnare ruoli AD a un gruppo cloud](https://docs.microsoft.com/azure/active-directory/roles/groups-concept). Per ulteriori informazioni sulla risoluzione dei problemi dei ruoli assegnati a gruppi cloud, vedere [Risoluzione dei problemi relativi ai ruoli assegnati a gruppi cloud](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).





