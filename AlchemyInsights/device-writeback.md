---
title: Writeback dei dispositivi
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "8279"
ms.openlocfilehash: f1a8dba19d220e1154549507801c813f56fe5cdd
ms.sourcegitcommit: 0470a728d184ceb89d1419f7ed57166e07bb778b
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 02/15/2021
ms.locfileid: "50255171"
---
# <a name="device-writeback"></a>Writeback dei dispositivi

Il writeback dei dispositivi viene utilizzato negli scenari seguenti:

- Abilitare [Windows Hello for Business con la distribuzione trust certificato ibrida](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)
- Abilitare l'accesso condizionale in base ai dispositivi alle applicazioni protette di ADFS (2012 R2 o versione successiva) (attendibilità relying party)

    > [!NOTE]
    > È necessaria una sottoscrizione ad Azure AD Premium per il writeback del dispositivo.

In questo modo si garantisce una sicurezza e una garanzia aggiuntive che l'accesso alle applicazioni viene concesso solo ai dispositivi attendibili. Per ulteriori informazioni sull'accesso condizionale, vedere [Gestione](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) dei rischi con l'accesso condizionale e Configurazione dell'accesso condizionale locale tramite la registrazione dei dispositivi [di Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/devices/overview)

Per altre informazioni sull'abilitazione del writeback dei dispositivi per i dispositivi, vedi [Abilitare il writeback dei dispositivi.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback)
