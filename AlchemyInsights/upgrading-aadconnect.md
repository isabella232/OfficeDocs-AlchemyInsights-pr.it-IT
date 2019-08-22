---
title: 932 aggiornamento di AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: ff3f74348599788edd8ce0991fe49bb6a54b55af
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36506087"
---
# <a name="upgrade-azure-ad-connect"></a>Aggiornamento di Azure AD Connect

Per impostazione predefinita, l'aggiornamento automatico è abilitato per Azure AD Connect, che consente di verificare che la versione più recente sia in esecuzione. Per verificare le impostazioni di aggiornamento automatico, utilizzare il cmdlet **Get-ADSyncAutoUpgrade** in Azure ad PowerShell. Il cmdlet restituirà uno dei seguenti valori:

- **Enabled**: l'aggiornamento automatico è abilitato.

- **Disabled**: l'aggiornamento automatico è disabilitato.

- **Sospesa**: il sistema non è più idoneo per ricevere gli aggiornamenti automatici. Non è possibile configurare questo valore. viene impostato dal sistema.

Per ulteriori informazioni, vedere [aggiornamento automatico](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Per scaricare la versione più recente di Azure AD Connect, passare [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594)a.
