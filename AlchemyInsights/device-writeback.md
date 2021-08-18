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
ms.openlocfilehash: c069d0b4588e53250d6cc1f3a66c744ea5c12ae4
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320090"
---
# <a name="device-writeback"></a>Writeback dei dispositivi

Il writeback dei dispositivi viene utilizzato negli scenari seguenti:

- Abilitare [Windows Hello per le aziende usando la distribuzione ibrida del certificato attendibile](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)
- Abilitare l'accesso condizionale in base ai dispositivi alle applicazioni protette con ADFS (2012 R2 o versione successiva) (attendibilità relying party)

    **Nota:** è necessaria una sottoscrizione Azure AD Premium per il writeback del dispositivo.

In questo modo si garantisce che l'accesso alle applicazioni sia concesso solo ai dispositivi attendibili. Per ulteriori informazioni sull'accesso condizionale, vedere [Managing Risk with Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) e Setting up [On-premises Conditional Access using Azure Active Directory Device Registration](https://docs.microsoft.com/azure/active-directory/devices/overview).

Per altre informazioni sull'abilitazione del writeback dei dispositivi per i dispositivi, vedi [Abilitare il writeback dei dispositivi.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback)
