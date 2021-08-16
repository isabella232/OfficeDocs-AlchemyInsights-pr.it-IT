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
ms.openlocfilehash: 78af4dc8cfe38586dcec8d01b72170b56d98fa27860489bf2ca9544f32210c37
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101954"
---
# <a name="device-writeback"></a>Writeback dei dispositivi

Il writeback dei dispositivi viene utilizzato negli scenari seguenti:

- Abilitare [Windows Hello per le aziende usando la distribuzione ibrida del certificato attendibile](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)
- Abilitare l'accesso condizionale in base ai dispositivi alle applicazioni protette con ADFS (2012 R2 o versione successiva) (attendibilità relying party)

    > [!NOTE]
    > È necessaria una sottoscrizione Azure AD Premium per il writeback del dispositivo.

In questo modo si garantisce che l'accesso alle applicazioni sia concesso solo ai dispositivi attendibili. Per ulteriori informazioni sull'accesso condizionale, vedere [Managing Risk with Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) e Setting up [On-premises Conditional Access using Azure Active Directory Device Registration](https://docs.microsoft.com/azure/active-directory/devices/overview).

Per altre informazioni sull'abilitazione del writeback dei dispositivi per i dispositivi, vedi [Abilitare il writeback dei dispositivi.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback)
