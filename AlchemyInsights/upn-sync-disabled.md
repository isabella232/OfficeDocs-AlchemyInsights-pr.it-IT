---
title: Sincronizzazione UPN disattivata
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: f390d659b191fa4c44bd7c8acb32409cd3021489
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36532335"
---
# <a name="upn-sync-disabled"></a>Sincronizzazione UPN disattivata

Se è stata avviata la sincronizzazione con Azure AD prima del 30 marzo 2016, eseguire il seguente cmdlet di Azure AD PowerShell per abilitare la corrispondenza morbida UPN solo per l'organizzazione:
  
 **Set-MsolDirSyncFeature-feature EnableSoftMatchOnUpn-Enable $True**
  
La combinazione di tasti UPN è attivata automaticamente per le organizzazioni che hanno iniziato a eseguire la sincronizzazione con Azure AD o dopo il 30 marzo 2016.
  
Per ulteriori informazioni sull'abilitazione della corrispondenza morbida su UPN e altre funzionalità di sincronizzazione, vedere [Azure ad Connect Sync Service Features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

