---
title: Aggiungere un gruppo a un sito di SharePoint
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 5dab9fce935936898927afd55f8f6e9260249157
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582815"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Problemi durante la creazione di un sito collegato a un gruppo in SharePoint

1. Alcuni problemi comuni riscontrati durante la creazione o la ricreazione di un sito collegato a un gruppo.
Se è stato eliminato un gruppo e il relativo sito connesso e si desidera creare un altro sito con lo stesso URL, è necessario rimuovere definitivamente il sito precedente.

   - Scaricare [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Per altre informazioni sulla Guida introduttiva a PowerShell, vedere [Guida introduttiva a SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - Rimuovere il sito dai siti eliminati utilizzando il cmdlet [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) di PowerShell. PowerShell è necessario per eliminare definitivamente i siti del gruppo.

1. Se si sta creando un sito collegato a un gruppo e viene visualizzato un messaggio di avviso: **esiste già un altro gruppo con lo stesso alias**, controllare i gruppi esistenti dall'interfaccia di [amministrazione di Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups). Per risolvere il problema, eliminare il gruppo esistente se non è più necessario o creare il sito con un altro alias assegnato.

1. Esistono diversi modi per creare e utilizzare i gruppi moderni con SharePoint.

   - È possibile connettere i siti esistenti a un gruppo di Microsoft 365. Per altre informazioni, vedere [connettere un gruppo di Microsoft 365 utilizzando l'interfaccia utente di SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Per creare un sito collegato a un gruppo di Microsoft 365, è necessario creare un [sito del team](https://admin.microsoft.com/sharepoint).
