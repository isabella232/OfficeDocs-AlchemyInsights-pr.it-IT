---
title: Sincronizzazione UPN disabilitata
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: fc163fae4d348d7c7cf117bd457f999b42f96bec7c1eb9aa1435e346131d06de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038116"
---
# <a name="upn-sync-disabled"></a>Sincronizzazione UPN disabilitata

Se è stata avviata la sincronizzazione con Azure AD prima del 30 marzo 2016, eseguire il cmdlet di Azure AD PowerShell seguente per abilitare la corrispondenza soft UPN solo per l'organizzazione:
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**
  
UpN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.
  
Per altre informazioni sull'abilitazione della corrispondenza soft su UPN e altre funzionalità di sincronizzazione, vedere Funzionalità del servizio di sincronizzazione di [Azure AD Connessione.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)
  

