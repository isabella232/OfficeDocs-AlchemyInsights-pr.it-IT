---
title: Codice di errore 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Se si è ricevuto un errore durante l'attivazione di Office 2013 in distribuzioni Remote Desktop Services (RDS), è possibile attivare ADAL modificando il Registro di sistema.
ms.openlocfilehash: 89f9270169e13fd7706f7826c624ef8ae4d47b3f
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/15/2019
ms.locfileid: "28296365"
---
Se si è ricevuto un errore durante l'attivazione di Office 2013 in distribuzioni Remote Desktop Services (RDS), è possibile attivare ADAL modificando il Registro di sistema. 
  
|**Chiave del Registro di sistema**|**Tipo**|**Valore**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |
   
Per ulteriori informazioni, vedere [Abilitare moderno Authentication for Office 2013 su dispositivi Windows.](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication)
  
> [!NOTE]
>  ADAL è abilitata per impostazione predefinita in Office 365 ProPlus e Office 2016. > Remote Desktop Services (RDS) è stato denominato in precedenza Servizi Terminal. 
  

