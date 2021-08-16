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
ms.openlocfilehash: 7eb3fd34ec6f1a2d431ed276b00dd46b5ec6aa73d69b37ef88b1ba0ca6f5d077
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54019188"
---
# <a name="block-user-from-recording-meetings"></a>Impedire all'utente di registrare riunioni

Se è necessario impedire **o impedire** a utenti specifici di registrare Teams riunioni, è possibile farlo Teams impostazioni dei criteri riunione. Nell'Microsoft Teams di amministrazione, disattivare l'impostazione Consenti registrazione **cloud** nel criterio riunione assegnato a tale utente. Per ulteriori informazioni, vedere [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-cloud-recording).

Per verificare se a un utente specifico è consentito o meno registrare Teams riunioni, utilizzare la diagnostica di supporto. Eseguire una nuova query di supporto e digitare **Diag: Registrazione** riunione: la diagnostica controlla le impostazioni dei criteri per l'utente specificato e ne determina le impostazioni. Tenere presente che l'applicazione delle nuove impostazioni dei criteri può richiedere un paio d'ore, quindi se è stata appena apportata una modifica, attendere alcune ore prima di eseguire di nuovo la diagnostica.

Per ulteriori informazioni, vedere [Attivare o disattivare la registrazione cloud.](https://docs.microsoft.com/microsoftteams/cloud-recording#turn-on-or-turn-off-cloud-recording)
