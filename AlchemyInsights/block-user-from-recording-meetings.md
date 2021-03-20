---
title: Impedire all'utente di registrare riunioni
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
- "9002530"
- "9325"
ms.openlocfilehash: 3f633ee1fb3329b6fc634acabbc824af1eccfb33
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897980"
---
# <a name="block-user-from-recording-meetings"></a>Impedire all'utente di registrare riunioni

Se è necessario impedire **o impedire** a utenti specifici di registrare riunioni di Teams, è possibile farlo tramite le impostazioni dei criteri riunione di Teams. Nell'interfaccia di amministrazione di Microsoft Teams disattivare l'impostazione Consenti registrazione **cloud** nel criterio riunione assegnato a tale utente. Per ulteriori informazioni, vedere [Manage meeting policies in Teams.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-cloud-recording)

Per verificare se a un utente specifico è consentito o meno registrare riunioni di Teams, utilizzare la diagnostica di supporto. Eseguire una nuova query di supporto e digitare **Diag: Registrazione** riunione: la diagnostica controlla le impostazioni dei criteri per l'utente specificato e ne determina le impostazioni. Tenere presente che l'applicazione delle nuove impostazioni dei criteri può richiedere un paio d'ore, quindi se è stata appena apportata una modifica, attendere alcune ore prima di eseguire di nuovo la diagnostica.

Per ulteriori informazioni, vedere [Attivare o disattivare la registrazione cloud.](https://docs.microsoft.com/microsoftteams/cloud-recording#turn-on-or-turn-off-cloud-recording)
