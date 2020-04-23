---
title: 932 aggiornamento di AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: fcc5fddb5cfd15407d0533449035317d187931ed
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766497"
---
# <a name="upgrade-azure-ad-connect"></a>Aggiornamento di Azure AD Connect

Per impostazione predefinita, l'aggiornamento automatico è abilitato per Azure AD Connect, che consente di verificare che la versione più recente sia in esecuzione. Per verificare le impostazioni di aggiornamento automatico, utilizzare il cmdlet **Get-ADSyncAutoUpgrade** in Azure ad PowerShell. Il cmdlet restituirà uno dei seguenti valori:

- **Enabled**: l'aggiornamento automatico è abilitato.

- **Disabled**: l'aggiornamento automatico è disabilitato.

- **Sospesa**: il sistema non è più idoneo per ricevere gli aggiornamenti automatici. Non è possibile configurare questo valore. viene impostato dal sistema.

Per ulteriori informazioni, vedere [aggiornamento automatico](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Per scaricare la versione più recente di Azure AD Connect, passare [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594)a.
