---
title: 932 aggiornamento di AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 932
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 8ffa8f64019077034bc4fad61d1d843849c42898
ms.sourcegitcommit: 1a4b8fa9e38a95ca811085af516edb81caf2018c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/13/2019
ms.locfileid: "31858964"
---
# <a name="upgrade-azure-ad-connect"></a>Aggiornamento di Azure AD Connect

Per impostazione predefinita, l'aggiornamento automatico è abilitato per Azure AD Connect, che consente di verificare che la versione più recente sia in esecuzione. Per verificare le impostazioni di aggiornamento automatico, utilizzare il cmdlet **Get-ADSyncAutoUpgrade** in Azure ad PowerShell. Il cmdlet restituirà uno dei seguenti valori: 

- **Enabled**: l'aggiornamento automatico è abilitato.

- **Disabled**: l'aggiornamento automatico è disabilitato.

- **Sospesa**: il sistema non è più idoneo per ricevere gli aggiornamenti automatici. Non è possibile configurare questo valore. viene impostato dal sistema. 

Per ulteriori informazioni, vedere [aggiornamento automatico](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Per scaricare la versione più recente di Azure AD Connect, passare [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594)a.
