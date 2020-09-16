---
title: Sincronizzazione UPN disattivata
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 31947d7c491e4116ffdb9baadf286cd4fbb50f2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749518"
---
# <a name="upn-sync-disabled"></a>Sincronizzazione UPN disattivata

Se è stata avviata la sincronizzazione con Azure AD prima del 30 marzo 2016, eseguire il seguente cmdlet di Azure AD PowerShell per abilitare la corrispondenza morbida UPN solo per l'organizzazione:
  
 **Set-MsolDirSyncFeature-feature EnableSoftMatchOnUpn-Enable $True**
  
La combinazione di tasti UPN è attivata automaticamente per le organizzazioni che hanno iniziato a eseguire la sincronizzazione con Azure AD o dopo il 30 marzo 2016.
  
Per ulteriori informazioni sull'abilitazione della corrispondenza morbida su UPN e altre funzionalità di sincronizzazione, vedere [Azure ad Connect Sync Service Features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

