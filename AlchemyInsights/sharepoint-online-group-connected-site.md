---
title: Aggiungere un gruppo a un SharePoint sito
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200004"
- "5766"
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 5dd159b8b9e141c2fb448bae5fb624efe1014d7d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58318128"
---
# <a name="common-issues-when-creating-a-group-connected-site-in-sharepoint"></a>Problemi comuni durante la creazione di un sito connesso a un gruppo in SharePoint

1. Se è stato eliminato un gruppo e il relativo sito connesso e si desidera creare un altro sito con lo stesso URL, sarà necessario rimuovere definitivamente il sito precedente.

   - Scaricare [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Per altre info su come iniziare a usare PowerShell, vedi Introduzione a [SharePoint Online Management Shell.](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite)
   - Rimuovere il sito dai siti eliminati utilizzando il cmdlet [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) di PowerShell. Powershell è necessario per eliminare definitivamente i siti di gruppo.

1. Se si sta creando un sito connesso a un gruppo e viene visualizzato [un avviso:](https://admin.microsoft.com/AdminPortal/Home#/groups)Esiste già un altro gruppo con lo stesso **alias,** controllare i gruppi esistenti dal interfaccia di amministrazione di Microsoft 365 . Per risolvere il problema, eliminare il gruppo esistente se non è più necessario o creare il sito con un alias diverso assegnato.

1. Esistono diversi modi per creare e usare gruppi moderni con SharePoint.

   - È possibile connettere siti esistenti a un Microsoft 365 gruppo. Per altre info, vedi [Connessione gruppo Microsoft 365 usando l'SharePoint utente](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Per creare un Microsoft 365 di gruppo connesso, è necessario creare un [sito del team.](https://admin.microsoft.com/sharepoint)
