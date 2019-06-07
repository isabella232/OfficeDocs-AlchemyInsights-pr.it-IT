---
title: Aggiungere un gruppo a un sito di SharePoint
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: f0126f7f753275e9bbf8c3a09a6af5faf9a27862
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/07/2019
ms.locfileid: "34758735"
---
# <a name="create-group-connected-site-in-sharepoint-online"></a>Creare un sito connesso a un gruppo in SharePoint Online

Durante la creazione o la ricreazione di un sito collegato a un gruppo sono stati riscontrati un paio di problemi comuni.

 Se è stato eliminato un gruppo e il relativo sito connesso e si desidera creare un altro sito con lo stesso URL, è necessario rimuovere definitivamente il sito precedente.

Scaricare [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)

 Per altre informazioni sulla Guida introduttiva a PowerShell, vedere [Guida introduttiva a SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)

Rimuovere il sito dai siti eliminati utilizzando il cmdlet [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) di PowerShell.

Se si sta creando un sito collegato a un gruppo e si riceve un avviso un altro gruppo con lo stesso alias esiste già, controllare i gruppi esistenti dall'interfaccia di [amministrazione di Office 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups). Per risolvere il problema, eliminare il gruppo esistente se non è più necessario o creare il sito con un altro alias assegnato.

Esistono diversi modi per creare e utilizzare i gruppi moderni con SharePoint.

È possibile connettere i siti esistenti a un gruppo di Office 365. Per altre informazioni, vedere [connettere un gruppo di Office 365 utilizzando l'utente di ineterface di SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).

Per creare un sito collegato a un gruppo di Office 365, è necessario creare un sito del team. Per altre informazioni, vedere [creare un sito del team in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).

