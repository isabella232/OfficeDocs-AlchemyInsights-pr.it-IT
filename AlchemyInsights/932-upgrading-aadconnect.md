---
title: 932 AADConnect l'aggiornamento
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 9add88a0e4a2590639cbfc546afdcdf5e6aa4886
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/15/2019
ms.locfileid: "28296622"
---
# <a name="upgrade-azure-ad-connect"></a>Connettere l'aggiornamento Azure Active Directory

Per impostazione predefinita, l'aggiornamento automatico è abilitata per Azure Active Directory Connect, che consente di verificare che è in esecuzione la versione più recente. Per verificare le impostazioni di aggiornamento automatiche, utilizzare il cmdlet **Get-ADSyncAutoUpgrade** in PowerShell di Azure Active Directory. Il cmdlet restituisce uno dei valori seguenti: 
  
- **Enabled**: l'aggiornamento automatico è attivato. 
    
- **Disabilitata**: l'aggiornamento automatico è disattivato. 
    
- **Suspended**: il sistema non è più idoneo ricevere aggiornamenti automatici. Non è possibile configurare questo valore. è impostato dal sistema. 
    
Per ulteriori informazioni, vedere [aggiornamento automatico](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).
  
Per scaricare la versione più recente di Azure Active Directory Connect, accedere a [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).
  

