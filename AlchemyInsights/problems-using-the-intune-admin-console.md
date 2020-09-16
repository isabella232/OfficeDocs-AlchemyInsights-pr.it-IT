---
title: Problemi nell’utilizzo della console di amministrazione di Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 10b37b2ffda50dc77396039a9e0e443ad81aef72
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728291"
---
# <a name="problems-using-the-intune-admin-console"></a>Problemi nell’utilizzo della console di amministrazione di Intune

**"Accesso negato" durante la navigazione nel portale di amministrazione di Intune.**

- Se si è membri di un ruolo personalizzato di Intune, assicurarsi che all'account sia assegnata una licenza di Intune o Enterprise Mobility Suite (EMS).
- Se si usa Configuration Manager per gestire i dispositivi, verificare di non far parte della raccolta di utenti di Intune per Configuration Manager MDM.
- Verificare che siano state assegnate le appropriate autorizzazioni di controllo di amministrazione in base al ruolo nel pannello dei ruoli di Intune.
- Verificare che il gruppo usato non sia una lista di distribuzione. Intune nel portale di Azure supporta solo gli account utente che appartengono a gruppi di sicurezza di Azure Active Directory. Controllare i gruppi nel portale di Azure > **Intune** > **Gruppi** o nel portale di Azure > **Azure Active Directory**.

**L’utente ha troppe autorizzazioni per il ruolo di Intune assegnato**

Consigliare all'utente di passare a **Intune** > **Ruoli di Intune** > **Autorizzazioni personali** > **Esportare** per rivedere le autorizzazioni concesse.

**È stato aggiunto un gruppo di ambito circoscritto a un ruolo, ma gli utenti in questo ruolo vedono ancora altri utenti o dispositivi.**

I gruppi di ambito circoscritto non filtrano utenti o dispositivi. Gruppi di ambito circoscritto:

- Limitano le persone alle quali gli utenti possono assegnare criteri o applicazioni.
- Consentono solo a specifici utenti di eseguire attività remote sui dispositivi.

Per altre informazioni sui gruppi di ambito circoscritto, vedere [Controllo degli accessi in base al ruolo (RBAC) con Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).

**È stato aggiunto un utente a un ruolo di Intune, ma è comunque possibile l’accesso completo alla console di amministrazione di Intune.**

Passare a Intune > **Utenti** nel portale di Azure e verificare che l'utente non sia assegnato ad alcuno dei ruoli seguenti nel portale di Azure:

- Amministratore globale
- Amministratore del servizio Intune
- Amministratore di SharePoint

Per altre informazioni, vedere [Controllo degli accessi in base al ruolo con Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).

**Problemi di accesso**

Per altre informazioni, vedere [Non è possibile accedere a Office 365, Azure o Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).