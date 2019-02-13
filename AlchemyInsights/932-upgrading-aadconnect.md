---
title: 932 AADConnect l'aggiornamento
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 8038d5ef768d6ee228db7d038ad71d926f4047f3
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29937948"
---
# <a name="upgrade-azure-ad-connect"></a>Connettere l'aggiornamento Azure Active Directory

Per impostazione predefinita, l'aggiornamento automatico è abilitata per Azure Active Directory Connect, che consente di verificare che è in esecuzione la versione più recente. Per verificare le impostazioni di aggiornamento automatiche, utilizzare il cmdlet **Get-ADSyncAutoUpgrade** in PowerShell di Azure Active Directory. Il cmdlet restituisce uno dei valori seguenti: 
  
- **Enabled**: l'aggiornamento automatico è attivato. 
    
- **Disabilitata**: l'aggiornamento automatico è disattivato. 
    
- **Suspended**: il sistema non è più idoneo ricevere aggiornamenti automatici. Non è possibile configurare questo valore. è impostato dal sistema. 
    
Per ulteriori informazioni, vedere [aggiornamento automatico](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).
  
Per scaricare la versione più recente di Azure Active Directory Connect, accedere a [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).
  

